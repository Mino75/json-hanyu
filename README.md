# json-hanyu
json-hanyu chinese character construction

This json file for MongoDB allos to describe the chinese characters link. Mongo allows to update.

without constructor :

                {   
                    "id":"口",
                    "strokes":"4",
                    "construct": [
                        "",
                    ]
                },

with constructor : 

                {   
                    "id":"呆",
                    "construct": [
                        {
                           "id":"木",
                           "recurrence" :"1",
                           "error-probability" : "0"

                        },
                        {
                            "id":"口",
                           "recurrence" :"1",
                           "error-probability" : "0"
                        }
                    ]
                },
                
               NEXT : caclulate the number of strokes, develop error probabilites with training models,
                
