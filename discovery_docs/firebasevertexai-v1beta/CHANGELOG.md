## 2025-04-19 21:27:30 UTC

**Summary:**
Could not generate summary (Gemini API key missing or call failed).

**Details (diff):**
```diff
--- /home/runner/work/_temp/old-discovery-formatted.json	2025-04-19 21:27:30.889175051 +0000
+++ /home/runner/work/_temp/new-discovery-formatted.json	2025-04-19 21:27:30.888175049 +0000
@@ -0,0 +1,2175 @@
+{
+  "description": "firebasevertexai.googleapis.com API.",
+  "icons": {
+    "x16": "http://www.google.com/images/icons/product/search-16.gif",
+    "x32": "http://www.google.com/images/icons/product/search-32.gif"
+  },
+  "auth": {
+    "oauth2": {
+      "scopes": {
+        "https://www.googleapis.com/auth/cloud-platform": {
+          "description": "See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account."
+        }
+      }
+    }
+  },
+  "version_module": true,
+  "baseUrl": "https://firebasevertexai.googleapis.com/",
+  "name": "firebasevertexai",
+  "resources": {
+    "projects": {
+      "resources": {
+        "locations": {
+          "resources": {
+            "publishers": {
+              "resources": {
+                "models": {
+                  "methods": {
+                    "predict": {
+                      "id": "firebasevertexai.projects.locations.publishers.models.predict",
+                      "path": "v1beta/{+endpoint}:predict",
+                      "flatPath": "v1beta/projects/{projectsId}/locations/{locationsId}/publishers/{publishersId}/models/{modelsId}:predict",
+                      "httpMethod": "POST",
+                      "parameters": {
+                        "endpoint": {
+                          "description": "Required. The name of the Endpoint requested to serve the prediction. Format: `projects/{project}/locations/{location}/endpoints/{endpoint}`",
+                          "pattern": "^projects/[^/]+/locations/[^/]+/publishers/[^/]+/models/[^/]+$",
+                          "location": "path",
+                          "required": true,
+                          "type": "string"
+                        }
+                      },
+                      "parameterOrder": [
+                        "endpoint"
+                      ],
+                      "request": {
+                        "$ref": "GoogleCloudAiplatformV1beta1PredictRequest"
+                      },
+                      "response": {
+                        "$ref": "GoogleCloudAiplatformV1beta1PredictResponse"
+                      },
+                      "scopes": [
+                        "https://www.googleapis.com/auth/cloud-platform"
+                      ],
+                      "description": "Perform an online prediction."
+                    },
+                    "countTokens": {
+                      "id": "firebasevertexai.projects.locations.publishers.models.countTokens",
+                      "path": "v1beta/{+endpoint}:countTokens",
+                      "flatPath": "v1beta/projects/{projectsId}/locations/{locationsId}/publishers/{publishersId}/models/{modelsId}:countTokens",
+                      "httpMethod": "POST",
+                      "parameters": {
+                        "endpoint": {
+                          "description": "Required. The name of the Endpoint requested to perform token counting. Format: `projects/{project}/locations/{location}/endpoints/{endpoint}`",
+                          "pattern": "^projects/[^/]+/locations/[^/]+/publishers/[^/]+/models/[^/]+$",
+                          "location": "path",
+                          "required": true,
+                          "type": "string"
+                        }
+                      },
+                      "parameterOrder": [
+                        "endpoint"
+                      ],
+                      "request": {
+                        "$ref": "GoogleCloudAiplatformV1beta1CountTokensRequest"
+                      },
+                      "response": {
+                        "$ref": "GoogleCloudAiplatformV1beta1CountTokensResponse"
+                      },
+                      "scopes": [
+                        "https://www.googleapis.com/auth/cloud-platform"
+                      ],
+                      "description": "Perform a token counting."
+                    },
+                    "generateContent": {
+                      "id": "firebasevertexai.projects.locations.publishers.models.generateContent",
+                      "path": "v1beta/{+model}:generateContent",
+                      "flatPath": "v1beta/projects/{projectsId}/locations/{locationsId}/publishers/{publishersId}/models/{modelsId}:generateContent",
+                      "httpMethod": "POST",
+                      "parameters": {
+                        "model": {
+                          "description": "Required. The fully qualified name of the publisher model or tuned model endpoint to use. Publisher model format: `projects/{project}/locations/{location}/publishers/*/models/*` Tuned model endpoint format: `projects/{project}/locations/{location}/endpoints/{endpoint}`",
+                          "pattern": "^projects/[^/]+/locations/[^/]+/publishers/[^/]+/models/[^/]+$",
+                          "location": "path",
+                          "required": true,
+                          "type": "string"
+                        }
+                      },
+                      "parameterOrder": [
+                        "model"
+                      ],
+                      "request": {
+                        "$ref": "GoogleCloudAiplatformV1beta1GenerateContentRequest"
+                      },
+                      "response": {
+                        "$ref": "GoogleCloudAiplatformV1beta1GenerateContentResponse"
+                      },
+                      "scopes": [
+                        "https://www.googleapis.com/auth/cloud-platform"
+                      ],
+                      "description": "Generate content with multimodal inputs."
+                    },
+                    "streamGenerateContent": {
+                      "id": "firebasevertexai.projects.locations.publishers.models.streamGenerateContent",
+                      "path": "v1beta/{+model}:streamGenerateContent",
+                      "flatPath": "v1beta/projects/{projectsId}/locations/{locationsId}/publishers/{publishersId}/models/{modelsId}:streamGenerateContent",
+                      "httpMethod": "POST",
+                      "parameters": {
+                        "model": {
+                          "description": "Required. The fully qualified name of the publisher model or tuned model endpoint to use. Publisher model format: `projects/{project}/locations/{location}/publishers/*/models/*` Tuned model endpoint format: `projects/{project}/locations/{location}/endpoints/{endpoint}`",
+                          "pattern": "^projects/[^/]+/locations/[^/]+/publishers/[^/]+/models/[^/]+$",
+                          "location": "path",
+                          "required": true,
+                          "type": "string"
+                        }
+                      },
+                      "parameterOrder": [
+                        "model"
+                      ],
+                      "request": {
+                        "$ref": "GoogleCloudAiplatformV1beta1GenerateContentRequest"
+                      },
+                      "response": {
+                        "$ref": "GoogleCloudAiplatformV1beta1GenerateContentResponse"
+                      },
+                      "scopes": [
+                        "https://www.googleapis.com/auth/cloud-platform"
+                      ],
+                      "description": "Generate content with multimodal inputs with streaming support."
+                    }
+                  }
+                }
+              }
+            }
+          }
+        }
+      }
+    }
+  },
+  "kind": "discovery#restDescription",
+  "discoveryVersion": "v1",
+  "basePath": "",
+  "ownerName": "Google",
+  "servicePath": "",
+  "protocol": "rest",
+  "canonicalName": "Firebase Vertex AI",
+  "mtlsRootUrl": "https://firebasevertexai.mtls.googleapis.com/",
+  "rootUrl": "https://firebasevertexai.googleapis.com/",
+  "schemas": {
+    "GoogleCloudAiplatformV1beta1PredictRequest": {
+      "id": "GoogleCloudAiplatformV1beta1PredictRequest",
+      "description": "Request message for PredictionService.Predict.",
+      "type": "object",
+      "properties": {
+        "instances": {
+          "description": "Required. The instances that are the input to the prediction call. A DeployedModel may have an upper limit on the number of instances it supports per request, and when it is exceeded the prediction call errors in case of AutoML Models, or, in case of customer created Models, the behaviour is as documented by that Model. The schema of any single instance may be specified via Endpoint's DeployedModels' Model's PredictSchemata's instance_schema_uri.",
+          "type": "array",
+          "items": {
+            "type": "any"
+          }
+        },
+        "parameters": {
+          "description": "The parameters that govern the prediction. The schema of the parameters may be specified via Endpoint's DeployedModels' Model's PredictSchemata's parameters_schema_uri.",
+          "type": "any"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1PredictResponse": {
+      "id": "GoogleCloudAiplatformV1beta1PredictResponse",
+      "description": "Response message for PredictionService.Predict.",
+      "type": "object",
+      "properties": {
+        "predictions": {
+          "description": "The predictions that are the output of the predictions call. The schema of any single prediction may be specified via Endpoint's DeployedModels' Model's PredictSchemata's prediction_schema_uri.",
+          "type": "array",
+          "items": {
+            "type": "any"
+          }
+        },
+        "deployedModelId": {
+          "description": "ID of the Endpoint's DeployedModel that served this prediction.",
+          "type": "string"
+        },
+        "model": {
+          "description": "Output only. The resource name of the Model which is deployed as the DeployedModel that this prediction hits.",
+          "readOnly": true,
+          "type": "string"
+        },
+        "modelVersionId": {
+          "description": "Output only. The version ID of the Model which is deployed as the DeployedModel that this prediction hits.",
+          "readOnly": true,
+          "type": "string"
+        },
+        "modelDisplayName": {
+          "description": "Output only. The display name of the Model which is deployed as the DeployedModel that this prediction hits.",
+          "readOnly": true,
+          "type": "string"
+        },
+        "metadata": {
+          "description": "Output only. Request-level metadata returned by the model. The metadata type will be dependent upon the model implementation.",
+          "readOnly": true,
+          "type": "any"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1CountTokensRequest": {
+      "id": "GoogleCloudAiplatformV1beta1CountTokensRequest",
+      "description": "Request message for PredictionService.CountTokens.",
+      "type": "object",
+      "properties": {
+        "model": {
+          "description": "Optional. The name of the publisher model requested to serve the prediction. Format: `projects/{project}/locations/{location}/publishers/*/models/*`",
+          "type": "string"
+        },
+        "instances": {
+          "description": "Optional. The instances that are the input to token counting call. Schema is identical to the prediction schema of the underlying model.",
+          "type": "array",
+          "items": {
+            "type": "any"
+          }
+        },
+        "contents": {
+          "description": "Optional. Input content.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1Content"
+          }
+        },
+        "systemInstruction": {
+          "description": "Optional. The user provided system instructions for the model. Note: only text should be used in parts and content in each part will be in a separate paragraph.",
+          "$ref": "GoogleCloudAiplatformV1beta1Content"
+        },
+        "tools": {
+          "description": "Optional. A list of `Tools` the model may use to generate the next response. A `Tool` is a piece of code that enables the system to interact with external systems to perform an action, or set of actions, outside of knowledge and scope of the model.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1Tool"
+          }
+        },
+        "generationConfig": {
+          "description": "Optional. Generation config that the model will use to generate the response.",
+          "$ref": "GoogleCloudAiplatformV1beta1GenerationConfig"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1Content": {
+      "id": "GoogleCloudAiplatformV1beta1Content",
+      "description": "The base structured datatype containing multi-part content of a message. A `Content` includes a `role` field designating the producer of the `Content` and a `parts` field containing multi-part data that contains the content of the message turn.",
+      "type": "object",
+      "properties": {
+        "role": {
+          "description": "Optional. The producer of the content. Must be either 'user' or 'model'. Useful to set for multi-turn conversations, otherwise can be left blank or unset.",
+          "type": "string"
+        },
+        "parts": {
+          "description": "Required. Ordered `Parts` that constitute a single message. Parts may have different IANA MIME types.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1Part"
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1Part": {
+      "id": "GoogleCloudAiplatformV1beta1Part",
+      "description": "A datatype containing media that is part of a multi-part `Content` message. A `Part` consists of data which has an associated datatype. A `Part` can only contain one of the accepted types in `Part.data`. A `Part` must have a fixed IANA MIME type identifying the type and subtype of the media if `inline_data` or `file_data` field is filled with raw bytes.",
+      "type": "object",
+      "properties": {
+        "text": {
+          "description": "Optional. Text part (can be code).",
+          "type": "string"
+        },
+        "inlineData": {
+          "description": "Optional. Inlined bytes data.",
+          "$ref": "GoogleCloudAiplatformV1beta1Blob"
+        },
+        "fileData": {
+          "description": "Optional. URI based data.",
+          "$ref": "GoogleCloudAiplatformV1beta1FileData"
+        },
+        "functionCall": {
+          "description": "Optional. A predicted [FunctionCall] returned from the model that contains a string representing the [FunctionDeclaration.name] with the parameters and their values.",
+          "$ref": "GoogleCloudAiplatformV1beta1FunctionCall"
+        },
+        "functionResponse": {
+          "description": "Optional. The result output of a [FunctionCall] that contains a string representing the [FunctionDeclaration.name] and a structured JSON object containing any output from the function call. It is used as context to the model.",
+          "$ref": "GoogleCloudAiplatformV1beta1FunctionResponse"
+        },
+        "executableCode": {
+          "description": "Optional. Code generated by the model that is meant to be executed.",
+          "$ref": "GoogleCloudAiplatformV1beta1ExecutableCode"
+        },
+        "codeExecutionResult": {
+          "description": "Optional. Result of executing the [ExecutableCode].",
+          "$ref": "GoogleCloudAiplatformV1beta1CodeExecutionResult"
+        },
+        "videoMetadata": {
+          "description": "Optional. Video metadata. The metadata should only be specified while the video data is presented in inline_data or file_data.",
+          "$ref": "GoogleCloudAiplatformV1beta1VideoMetadata"
+        },
+        "thought": {
+          "description": "Output only. Indicates if the part is thought from the model.",
+          "readOnly": true,
+          "type": "boolean"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1Blob": {
+      "id": "GoogleCloudAiplatformV1beta1Blob",
+      "description": "Content blob.",
+      "type": "object",
+      "properties": {
+        "mimeType": {
+          "description": "Required. The IANA standard MIME type of the source data.",
+          "type": "string"
+        },
+        "data": {
+          "description": "Required. Raw bytes.",
+          "type": "string",
+          "format": "byte"
+        },
+        "displayName": {
+          "description": "Optional. Display name of the blob. Used to provide a label or filename to distinguish blobs. This field is only returned in PromptMessage for prompt management. It is not currently used in the Gemini GenerateContent calls.",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1FileData": {
+      "id": "GoogleCloudAiplatformV1beta1FileData",
+      "description": "URI based data.",
+      "type": "object",
+      "properties": {
+        "mimeType": {
+          "description": "Required. The IANA standard MIME type of the source data.",
+          "type": "string"
+        },
+        "fileUri": {
+          "description": "Required. URI.",
+          "type": "string"
+        },
+        "displayName": {
+          "description": "Optional. Display name of the file data. Used to provide a label or filename to distinguish file datas. This field is only returned in PromptMessage for prompt management. It is not currently used in the Gemini GenerateContent calls.",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1FunctionCall": {
+      "id": "GoogleCloudAiplatformV1beta1FunctionCall",
+      "description": "A predicted [FunctionCall] returned from the model that contains a string representing the [FunctionDeclaration.name] and a structured JSON object containing the parameters and their values.",
+      "type": "object",
+      "properties": {
+        "id": {
+          "description": "Optional. The unique id of the function call. If populated, the client to execute the `function_call` and return the response with the matching `id`.",
+          "type": "string"
+        },
+        "name": {
+          "description": "Required. The name of the function to call. Matches [FunctionDeclaration.name].",
+          "type": "string"
+        },
+        "args": {
+          "description": "Optional. The function parameters and values in JSON object format. See [FunctionDeclaration.parameters] for parameter details.",
+          "type": "object",
+          "additionalProperties": {
+            "type": "any",
+            "description": "Properties of the object."
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1FunctionResponse": {
+      "id": "GoogleCloudAiplatformV1beta1FunctionResponse",
+      "description": "The result output from a [FunctionCall] that contains a string representing the [FunctionDeclaration.name] and a structured JSON object containing any output from the function is used as context to the model. This should contain the result of a [FunctionCall] made based on model prediction.",
+      "type": "object",
+      "properties": {
+        "id": {
+          "description": "Optional. The id of the function call this response is for. Populated by the client to match the corresponding function call `id`.",
+          "type": "string"
+        },
+        "name": {
+          "description": "Required. The name of the function to call. Matches [FunctionDeclaration.name] and [FunctionCall.name].",
+          "type": "string"
+        },
+        "response": {
+          "description": "Required. The function response in JSON object format. Use \"output\" key to specify function output and \"error\" key to specify error details (if any). If \"output\" and \"error\" keys are not specified, then whole \"response\" is treated as function output.",
+          "type": "object",
+          "additionalProperties": {
+            "type": "any",
+            "description": "Properties of the object."
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1ExecutableCode": {
+      "id": "GoogleCloudAiplatformV1beta1ExecutableCode",
+      "description": "Code generated by the model that is meant to be executed, and the result returned to the model. Generated when using the [FunctionDeclaration] tool and [FunctionCallingConfig] mode is set to [Mode.CODE].",
+      "type": "object",
+      "properties": {
+        "language": {
+          "description": "Required. Programming language of the `code`.",
+          "type": "string",
+          "enumDescriptions": [
+            "Unspecified language. This value should not be used.",
+            "Python >= 3.10, with numpy and simpy available."
+          ],
+          "enum": [
+            "LANGUAGE_UNSPECIFIED",
+            "PYTHON"
+          ]
+        },
+        "code": {
+          "description": "Required. The code to be executed.",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1CodeExecutionResult": {
+      "id": "GoogleCloudAiplatformV1beta1CodeExecutionResult",
+      "description": "Result of executing the [ExecutableCode]. Always follows a `part` containing the [ExecutableCode].",
+      "type": "object",
+      "properties": {
+        "outcome": {
+          "description": "Required. Outcome of the code execution.",
+          "type": "string",
+          "enumDescriptions": [
+            "Unspecified status. This value should not be used.",
+            "Code execution completed successfully.",
+            "Code execution finished but with a failure. `stderr` should contain the reason.",
+            "Code execution ran for too long, and was cancelled. There may or may not be a partial output present."
+          ],
+          "enum": [
+            "OUTCOME_UNSPECIFIED",
+            "OUTCOME_OK",
+            "OUTCOME_FAILED",
+            "OUTCOME_DEADLINE_EXCEEDED"
+          ]
+        },
+        "output": {
+          "description": "Optional. Contains stdout when code execution is successful, stderr or other description otherwise.",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1VideoMetadata": {
+      "id": "GoogleCloudAiplatformV1beta1VideoMetadata",
+      "description": "Metadata describes the input video content.",
+      "type": "object",
+      "properties": {
+        "startOffset": {
+          "description": "Optional. The start offset of the video.",
+          "type": "string",
+          "format": "google-duration"
+        },
+        "endOffset": {
+          "description": "Optional. The end offset of the video.",
+          "type": "string",
+          "format": "google-duration"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1Tool": {
+      "id": "GoogleCloudAiplatformV1beta1Tool",
+      "description": "Tool details that the model may use to generate response. A `Tool` is a piece of code that enables the system to interact with external systems to perform an action, or set of actions, outside of knowledge and scope of the model. A Tool object should contain exactly one type of Tool (e.g FunctionDeclaration, Retrieval or GoogleSearchRetrieval).",
+      "type": "object",
+      "properties": {
+        "functionDeclarations": {
+          "description": "Optional. Function tool type. One or more function declarations to be passed to the model along with the current user query. Model may decide to call a subset of these functions by populating FunctionCall in the response. User should provide a FunctionResponse for each function call in the next turn. Based on the function responses, Model will generate the final response back to the user. Maximum 128 function declarations can be provided.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1FunctionDeclaration"
+          }
+        },
+        "retrieval": {
+          "description": "Optional. Retrieval tool type. System will always execute the provided retrieval tool(s) to get external knowledge to answer the prompt. Retrieval results are presented to the model for generation.",
+          "$ref": "GoogleCloudAiplatformV1beta1Retrieval"
+        },
+        "googleSearch": {
+          "description": "Optional. GoogleSearch tool type. Tool to support Google Search in Model. Powered by Google.",
+          "$ref": "GoogleCloudAiplatformV1beta1ToolGoogleSearch"
+        },
+        "googleSearchRetrieval": {
+          "description": "Optional. GoogleSearchRetrieval tool type. Specialized retrieval tool that is powered by Google search.",
+          "$ref": "GoogleCloudAiplatformV1beta1GoogleSearchRetrieval"
+        },
+        "enterpriseWebSearch": {
+          "description": "Optional. Tool to support searching public web data, powered by Vertex AI Search and Sec4 compliance.",
+          "$ref": "GoogleCloudAiplatformV1beta1EnterpriseWebSearch"
+        },
+        "codeExecution": {
+          "description": "Optional. CodeExecution tool type. Enables the model to execute code as part of generation.",
+          "$ref": "GoogleCloudAiplatformV1beta1ToolCodeExecution"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1FunctionDeclaration": {
+      "id": "GoogleCloudAiplatformV1beta1FunctionDeclaration",
+      "description": "Structured representation of a function declaration as defined by the [OpenAPI 3.0 specification](https://spec.openapis.org/oas/v3.0.3). Included in this declaration are the function name, description, parameters and response type. This FunctionDeclaration is a representation of a block of code that can be used as a `Tool` by the model and executed by the client.",
+      "type": "object",
+      "properties": {
+        "name": {
+          "description": "Required. The name of the function to call. Must start with a letter or an underscore. Must be a-z, A-Z, 0-9, or contain underscores, dots and dashes, with a maximum length of 64.",
+          "type": "string"
+        },
+        "description": {
+          "description": "Optional. Description and purpose of the function. Model uses it to decide how and whether to call the function.",
+          "type": "string"
+        },
+        "parameters": {
+          "description": "Optional. Describes the parameters to this function in JSON Schema Object format. Reflects the Open API 3.03 Parameter Object. string Key: the name of the parameter. Parameter names are case sensitive. Schema Value: the Schema defining the type used for the parameter. For function with no parameters, this can be left unset. Parameter names must start with a letter or an underscore and must only contain chars a-z, A-Z, 0-9, or underscores with a maximum length of 64. Example with 1 required and 1 optional parameter: type: OBJECT properties: param1: type: STRING param2: type: INTEGER required: - param1",
+          "$ref": "GoogleCloudAiplatformV1beta1Schema"
+        },
+        "response": {
+          "description": "Optional. Describes the output from this function in JSON Schema format. Reflects the Open API 3.03 Response Object. The Schema defines the type used for the response value of the function.",
+          "$ref": "GoogleCloudAiplatformV1beta1Schema"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1Schema": {
+      "id": "GoogleCloudAiplatformV1beta1Schema",
+      "description": "Schema is used to define the format of input/output data. Represents a select subset of an [OpenAPI 3.0 schema object](https://spec.openapis.org/oas/v3.0.3#schema-object). More fields may be added in the future as needed.",
+      "type": "object",
+      "properties": {
+        "type": {
+          "description": "Optional. The type of the data.",
+          "type": "string",
+          "enumDescriptions": [
+            "Not specified, should not be used.",
+            "OpenAPI string type",
+            "OpenAPI number type",
+            "OpenAPI integer type",
+            "OpenAPI boolean type",
+            "OpenAPI array type",
+            "OpenAPI object type"
+          ],
+          "enum": [
+            "TYPE_UNSPECIFIED",
+            "STRING",
+            "NUMBER",
+            "INTEGER",
+            "BOOLEAN",
+            "ARRAY",
+            "OBJECT"
+          ]
+        },
+        "format": {
+          "description": "Optional. The format of the data. Supported formats: for NUMBER type: \"float\", \"double\" for INTEGER type: \"int32\", \"int64\" for STRING type: \"email\", \"byte\", etc",
+          "type": "string"
+        },
+        "title": {
+          "description": "Optional. The title of the Schema.",
+          "type": "string"
+        },
+        "description": {
+          "description": "Optional. The description of the data.",
+          "type": "string"
+        },
+        "nullable": {
+          "description": "Optional. Indicates if the value may be null.",
+          "type": "boolean"
+        },
+        "default": {
+          "description": "Optional. Default value of the data.",
+          "type": "any"
+        },
+        "items": {
+          "description": "Optional. SCHEMA FIELDS FOR TYPE ARRAY Schema of the elements of Type.ARRAY.",
+          "$ref": "GoogleCloudAiplatformV1beta1Schema"
+        },
+        "minItems": {
+          "description": "Optional. Minimum number of the elements for Type.ARRAY.",
+          "type": "string",
+          "format": "int64"
+        },
+        "maxItems": {
+          "description": "Optional. Maximum number of the elements for Type.ARRAY.",
+          "type": "string",
+          "format": "int64"
+        },
+        "enum": {
+          "description": "Optional. Possible values of the element of primitive type with enum format. Examples: 1. We can define direction as : {type:STRING, format:enum, enum:[\"EAST\", NORTH\", \"SOUTH\", \"WEST\"]} 2. We can define apartment number as : {type:INTEGER, format:enum, enum:[\"101\", \"201\", \"301\"]}",
+          "type": "array",
+          "items": {
+            "type": "string"
+          }
+        },
+        "properties": {
+          "description": "Optional. SCHEMA FIELDS FOR TYPE OBJECT Properties of Type.OBJECT.",
+          "type": "object",
+          "additionalProperties": {
+            "$ref": "GoogleCloudAiplatformV1beta1Schema"
+          }
+        },
+        "propertyOrdering": {
+          "description": "Optional. The order of the properties. Not a standard field in open api spec. Only used to support the order of the properties.",
+          "type": "array",
+          "items": {
+            "type": "string"
+          }
+        },
+        "required": {
+          "description": "Optional. Required properties of Type.OBJECT.",
+          "type": "array",
+          "items": {
+            "type": "string"
+          }
+        },
+        "minProperties": {
+          "description": "Optional. Minimum number of the properties for Type.OBJECT.",
+          "type": "string",
+          "format": "int64"
+        },
+        "maxProperties": {
+          "description": "Optional. Maximum number of the properties for Type.OBJECT.",
+          "type": "string",
+          "format": "int64"
+        },
+        "minimum": {
+          "description": "Optional. SCHEMA FIELDS FOR TYPE INTEGER and NUMBER Minimum value of the Type.INTEGER and Type.NUMBER",
+          "type": "number",
+          "format": "double"
+        },
+        "maximum": {
+          "description": "Optional. Maximum value of the Type.INTEGER and Type.NUMBER",
+          "type": "number",
+          "format": "double"
+        },
+        "minLength": {
+          "description": "Optional. SCHEMA FIELDS FOR TYPE STRING Minimum length of the Type.STRING",
+          "type": "string",
+          "format": "int64"
+        },
+        "maxLength": {
+          "description": "Optional. Maximum length of the Type.STRING",
+          "type": "string",
+          "format": "int64"
+        },
+        "pattern": {
+          "description": "Optional. Pattern of the Type.STRING to restrict a string to a regular expression.",
+          "type": "string"
+        },
+        "example": {
+          "description": "Optional. Example of the object. Will only populated when the object is the root.",
+          "type": "any"
+        },
+        "anyOf": {
+          "description": "Optional. The value should be validated against any (one or more) of the subschemas in the list.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1Schema"
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1Retrieval": {
+      "id": "GoogleCloudAiplatformV1beta1Retrieval",
+      "description": "Defines a retrieval tool that model can call to access external knowledge.",
+      "type": "object",
+      "properties": {
+        "vertexAiSearch": {
+          "description": "Set to use data source powered by Vertex AI Search.",
+          "$ref": "GoogleCloudAiplatformV1beta1VertexAISearch"
+        },
+        "vertexRagStore": {
+          "description": "Set to use data source powered by Vertex RAG store. User data is uploaded via the VertexRagDataService.",
+          "$ref": "GoogleCloudAiplatformV1beta1VertexRagStore"
+        },
+        "disableAttribution": {
+          "description": "Optional. Deprecated. This option is no longer supported.",
+          "deprecated": true,
+          "type": "boolean"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1VertexAISearch": {
+      "id": "GoogleCloudAiplatformV1beta1VertexAISearch",
+      "description": "Retrieve from Vertex AI Search datastore or engine for grounding. datastore and engine are mutually exclusive. See https://cloud.google.com/products/agent-builder",
+      "type": "object",
+      "properties": {
+        "datastore": {
+          "description": "Optional. Fully-qualified Vertex AI Search data store resource ID. Format: `projects/{project}/locations/{location}/collections/{collection}/dataStores/{dataStore}`",
+          "type": "string"
+        },
+        "engine": {
+          "description": "Optional. Fully-qualified Vertex AI Search engine resource ID. Format: `projects/{project}/locations/{location}/collections/{collection}/engines/{engine}`",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1VertexRagStore": {
+      "id": "GoogleCloudAiplatformV1beta1VertexRagStore",
+      "description": "Retrieve from Vertex RAG Store for grounding.",
+      "type": "object",
+      "properties": {
+        "ragCorpora": {
+          "description": "Optional. Deprecated. Please use rag_resources instead.",
+          "deprecated": true,
+          "type": "array",
+          "items": {
+            "type": "string"
+          }
+        },
+        "ragResources": {
+          "description": "Optional. The representation of the rag source. It can be used to specify corpus only or ragfiles. Currently only support one corpus or multiple files from one corpus. In the future we may open up multiple corpora support.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1VertexRagStoreRagResource"
+          }
+        },
+        "similarityTopK": {
+          "description": "Optional. Number of top k results to return from the selected corpora.",
+          "deprecated": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "vectorDistanceThreshold": {
+          "description": "Optional. Only return results with vector distance smaller than the threshold.",
+          "deprecated": true,
+          "type": "number",
+          "format": "double"
+        },
+        "ragRetrievalConfig": {
+          "description": "Optional. The retrieval config for the Rag query.",
+          "$ref": "GoogleCloudAiplatformV1beta1RagRetrievalConfig"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1VertexRagStoreRagResource": {
+      "id": "GoogleCloudAiplatformV1beta1VertexRagStoreRagResource",
+      "description": "The definition of the Rag resource.",
+      "type": "object",
+      "properties": {
+        "ragCorpus": {
+          "description": "Optional. RagCorpora resource name. Format: `projects/{project}/locations/{location}/ragCorpora/{rag_corpus}`",
+          "type": "string"
+        },
+        "ragFileIds": {
+          "description": "Optional. rag_file_id. The files should be in the same rag_corpus set in rag_corpus field.",
+          "type": "array",
+          "items": {
+            "type": "string"
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RagRetrievalConfig": {
+      "id": "GoogleCloudAiplatformV1beta1RagRetrievalConfig",
+      "description": "Specifies the context retrieval config.",
+      "type": "object",
+      "properties": {
+        "topK": {
+          "description": "Optional. The number of contexts to retrieve.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "hybridSearch": {
+          "description": "Optional. Config for Hybrid Search.",
+          "$ref": "GoogleCloudAiplatformV1beta1RagRetrievalConfigHybridSearch"
+        },
+        "filter": {
+          "description": "Optional. Config for filters.",
+          "$ref": "GoogleCloudAiplatformV1beta1RagRetrievalConfigFilter"
+        },
+        "ranking": {
+          "description": "Optional. Config for ranking and reranking.",
+          "$ref": "GoogleCloudAiplatformV1beta1RagRetrievalConfigRanking"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RagRetrievalConfigHybridSearch": {
+      "id": "GoogleCloudAiplatformV1beta1RagRetrievalConfigHybridSearch",
+      "description": "Config for Hybrid Search.",
+      "type": "object",
+      "properties": {
+        "alpha": {
+          "description": "Optional. Alpha value controls the weight between dense and sparse vector search results. The range is [0, 1], while 0 means sparse vector search only and 1 means dense vector search only. The default value is 0.5 which balances sparse and dense vector search equally.",
+          "type": "number",
+          "format": "float"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RagRetrievalConfigFilter": {
+      "id": "GoogleCloudAiplatformV1beta1RagRetrievalConfigFilter",
+      "description": "Config for filters.",
+      "type": "object",
+      "properties": {
+        "vectorDistanceThreshold": {
+          "description": "Optional. Only returns contexts with vector distance smaller than the threshold.",
+          "type": "number",
+          "format": "double"
+        },
+        "vectorSimilarityThreshold": {
+          "description": "Optional. Only returns contexts with vector similarity larger than the threshold.",
+          "type": "number",
+          "format": "double"
+        },
+        "metadataFilter": {
+          "description": "Optional. String for metadata filtering.",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RagRetrievalConfigRanking": {
+      "id": "GoogleCloudAiplatformV1beta1RagRetrievalConfigRanking",
+      "description": "Config for ranking and reranking.",
+      "type": "object",
+      "properties": {
+        "rankService": {
+          "description": "Optional. Config for Rank Service.",
+          "$ref": "GoogleCloudAiplatformV1beta1RagRetrievalConfigRankingRankService"
+        },
+        "llmRanker": {
+          "description": "Optional. Config for LlmRanker.",
+          "$ref": "GoogleCloudAiplatformV1beta1RagRetrievalConfigRankingLlmRanker"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RagRetrievalConfigRankingRankService": {
+      "id": "GoogleCloudAiplatformV1beta1RagRetrievalConfigRankingRankService",
+      "description": "Config for Rank Service.",
+      "type": "object",
+      "properties": {
+        "modelName": {
+          "description": "Optional. The model name of the rank service. Format: `semantic-ranker-512@latest`",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RagRetrievalConfigRankingLlmRanker": {
+      "id": "GoogleCloudAiplatformV1beta1RagRetrievalConfigRankingLlmRanker",
+      "description": "Config for LlmRanker.",
+      "type": "object",
+      "properties": {
+        "modelName": {
+          "description": "Optional. The model name used for ranking. See [Supported models](https://cloud.google.com/vertex-ai/generative-ai/docs/model-reference/inference#supported-models).",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1ToolGoogleSearch": {
+      "id": "GoogleCloudAiplatformV1beta1ToolGoogleSearch",
+      "description": "GoogleSearch tool type. Tool to support Google Search in Model. Powered by Google.",
+      "type": "object",
+      "properties": {}
+    },
+    "GoogleCloudAiplatformV1beta1GoogleSearchRetrieval": {
+      "id": "GoogleCloudAiplatformV1beta1GoogleSearchRetrieval",
+      "description": "Tool to retrieve public web data for grounding, powered by Google.",
+      "type": "object",
+      "properties": {
+        "dynamicRetrievalConfig": {
+          "description": "Specifies the dynamic retrieval configuration for the given source.",
+          "$ref": "GoogleCloudAiplatformV1beta1DynamicRetrievalConfig"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1DynamicRetrievalConfig": {
+      "id": "GoogleCloudAiplatformV1beta1DynamicRetrievalConfig",
+      "description": "Describes the options to customize dynamic retrieval.",
+      "type": "object",
+      "properties": {
+        "mode": {
+          "description": "The mode of the predictor to be used in dynamic retrieval.",
+          "type": "string",
+          "enumDescriptions": [
+            "Always trigger retrieval.",
+            "Run retrieval only when system decides it is necessary."
+          ],
+          "enum": [
+            "MODE_UNSPECIFIED",
+            "MODE_DYNAMIC"
+          ]
+        },
+        "dynamicThreshold": {
+          "description": "Optional. The threshold to be used in dynamic retrieval. If not set, a system default value is used.",
+          "type": "number",
+          "format": "float"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1EnterpriseWebSearch": {
+      "id": "GoogleCloudAiplatformV1beta1EnterpriseWebSearch",
+      "description": "Tool to search public web data, powered by Vertex AI Search and Sec4 compliance.",
+      "type": "object",
+      "properties": {}
+    },
+    "GoogleCloudAiplatformV1beta1ToolCodeExecution": {
+      "id": "GoogleCloudAiplatformV1beta1ToolCodeExecution",
+      "description": "Tool that executes code generated by the model, and automatically returns the result to the model. See also [ExecutableCode]and [CodeExecutionResult] which are input and output to this tool.",
+      "type": "object",
+      "properties": {}
+    },
+    "GoogleCloudAiplatformV1beta1GenerationConfig": {
+      "id": "GoogleCloudAiplatformV1beta1GenerationConfig",
+      "description": "Generation config.",
+      "type": "object",
+      "properties": {
+        "temperature": {
+          "description": "Optional. Controls the randomness of predictions.",
+          "type": "number",
+          "format": "float"
+        },
+        "topP": {
+          "description": "Optional. If specified, nucleus sampling will be used.",
+          "type": "number",
+          "format": "float"
+        },
+        "topK": {
+          "description": "Optional. If specified, top-k sampling will be used.",
+          "type": "number",
+          "format": "float"
+        },
+        "candidateCount": {
+          "description": "Optional. Number of candidates to generate.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "maxOutputTokens": {
+          "description": "Optional. The maximum number of output tokens to generate per message.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "stopSequences": {
+          "description": "Optional. Stop sequences.",
+          "type": "array",
+          "items": {
+            "type": "string"
+          }
+        },
+        "responseLogprobs": {
+          "description": "Optional. If true, export the logprobs results in response.",
+          "type": "boolean"
+        },
+        "logprobs": {
+          "description": "Optional. Logit probabilities.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "presencePenalty": {
+          "description": "Optional. Positive penalties.",
+          "type": "number",
+          "format": "float"
+        },
+        "frequencyPenalty": {
+          "description": "Optional. Frequency penalties.",
+          "type": "number",
+          "format": "float"
+        },
+        "seed": {
+          "description": "Optional. Seed.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "responseMimeType": {
+          "description": "Optional. Output response mimetype of the generated candidate text. Supported mimetype: - `text/plain`: (default) Text output. - `application/json`: JSON response in the candidates. The model needs to be prompted to output the appropriate response type, otherwise the behavior is undefined. This is a preview feature.",
+          "type": "string"
+        },
+        "responseSchema": {
+          "description": "Optional. The `Schema` object allows the definition of input and output data types. These types can be objects, but also primitives and arrays. Represents a select subset of an [OpenAPI 3.0 schema object](https://spec.openapis.org/oas/v3.0.3#schema). If set, a compatible response_mime_type must also be set. Compatible mimetypes: `application/json`: Schema for JSON response.",
+          "$ref": "GoogleCloudAiplatformV1beta1Schema"
+        },
+        "routingConfig": {
+          "description": "Optional. Routing configuration.",
+          "$ref": "GoogleCloudAiplatformV1beta1GenerationConfigRoutingConfig"
+        },
+        "audioTimestamp": {
+          "description": "Optional. If enabled, audio timestamp will be included in the request to the model.",
+          "type": "boolean"
+        },
+        "responseModalities": {
+          "description": "Optional. The modalities of the response.",
+          "type": "array",
+          "items": {
+            "type": "string",
+            "enumDescriptions": [
+              "Unspecified modality. Will be processed as text.",
+              "Text modality.",
+              "Image modality.",
+              "Audio modality."
+            ],
+            "enum": [
+              "MODALITY_UNSPECIFIED",
+              "TEXT",
+              "IMAGE",
+              "AUDIO"
+            ]
+          }
+        },
+        "mediaResolution": {
+          "description": "Optional. If specified, the media resolution specified will be used.",
+          "type": "string",
+          "enumDescriptions": [
+            "Media resolution has not been set.",
+            "Media resolution set to low (64 tokens).",
+            "Media resolution set to medium (256 tokens).",
+            "Media resolution set to high (zoomed reframing with 256 tokens)."
+          ],
+          "enum": [
+            "MEDIA_RESOLUTION_UNSPECIFIED",
+            "MEDIA_RESOLUTION_LOW",
+            "MEDIA_RESOLUTION_MEDIUM",
+            "MEDIA_RESOLUTION_HIGH"
+          ]
+        },
+        "speechConfig": {
+          "description": "Optional. The speech generation config.",
+          "$ref": "GoogleCloudAiplatformV1beta1SpeechConfig"
+        },
+        "thinkingConfig": {
+          "description": "Optional. Config for thinking features. An error will be returned if this field is set for models that don't support thinking.",
+          "$ref": "GoogleCloudAiplatformV1beta1GenerationConfigThinkingConfig"
+        },
+        "modelConfig": {
+          "description": "Optional. Config for model selection.",
+          "$ref": "GoogleCloudAiplatformV1beta1GenerationConfigModelConfig"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GenerationConfigRoutingConfig": {
+      "id": "GoogleCloudAiplatformV1beta1GenerationConfigRoutingConfig",
+      "description": "The configuration for routing the request to a specific model.",
+      "type": "object",
+      "properties": {
+        "autoMode": {
+          "description": "Automated routing.",
+          "$ref": "GoogleCloudAiplatformV1beta1GenerationConfigRoutingConfigAutoRoutingMode"
+        },
+        "manualMode": {
+          "description": "Manual routing.",
+          "$ref": "GoogleCloudAiplatformV1beta1GenerationConfigRoutingConfigManualRoutingMode"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GenerationConfigRoutingConfigAutoRoutingMode": {
+      "id": "GoogleCloudAiplatformV1beta1GenerationConfigRoutingConfigAutoRoutingMode",
+      "description": "When automated routing is specified, the routing will be determined by the pretrained routing model and customer provided model routing preference.",
+      "type": "object",
+      "properties": {
+        "modelRoutingPreference": {
+          "description": "The model routing preference.",
+          "type": "string",
+          "enumDescriptions": [
+            "Unspecified model routing preference.",
+            "Prefer higher quality over low cost.",
+            "Balanced model routing preference.",
+            "Prefer lower cost over higher quality."
+          ],
+          "enum": [
+            "UNKNOWN",
+            "PRIORITIZE_QUALITY",
+            "BALANCED",
+            "PRIORITIZE_COST"
+          ]
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GenerationConfigRoutingConfigManualRoutingMode": {
+      "id": "GoogleCloudAiplatformV1beta1GenerationConfigRoutingConfigManualRoutingMode",
+      "description": "When manual routing is set, the specified model will be used directly.",
+      "type": "object",
+      "properties": {
+        "modelName": {
+          "description": "The model name to use. Only the public LLM models are accepted. See [Supported models](https://cloud.google.com/vertex-ai/generative-ai/docs/model-reference/inference#supported-models).",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1SpeechConfig": {
+      "id": "GoogleCloudAiplatformV1beta1SpeechConfig",
+      "description": "The speech generation config.",
+      "type": "object",
+      "properties": {
+        "voiceConfig": {
+          "description": "The configuration for the speaker to use.",
+          "$ref": "GoogleCloudAiplatformV1beta1VoiceConfig"
+        },
+        "languageCode": {
+          "description": "Optional. Language code (ISO 639. e.g. en-US) for the speech synthesization.",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1VoiceConfig": {
+      "id": "GoogleCloudAiplatformV1beta1VoiceConfig",
+      "description": "The configuration for the voice to use.",
+      "type": "object",
+      "properties": {
+        "prebuiltVoiceConfig": {
+          "description": "The configuration for the prebuilt voice to use.",
+          "$ref": "GoogleCloudAiplatformV1beta1PrebuiltVoiceConfig"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1PrebuiltVoiceConfig": {
+      "id": "GoogleCloudAiplatformV1beta1PrebuiltVoiceConfig",
+      "description": "The configuration for the prebuilt speaker to use.",
+      "type": "object",
+      "properties": {
+        "voiceName": {
+          "description": "The name of the preset voice to use.",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GenerationConfigThinkingConfig": {
+      "id": "GoogleCloudAiplatformV1beta1GenerationConfigThinkingConfig",
+      "description": "Config for thinking features.",
+      "type": "object",
+      "properties": {
+        "thinkingBudget": {
+          "description": "Optional. Indicates the thinking budget in tokens. This is only applied when enable_thinking is true.",
+          "type": "integer",
+          "format": "int32"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GenerationConfigModelConfig": {
+      "id": "GoogleCloudAiplatformV1beta1GenerationConfigModelConfig",
+      "description": "Config for model selection.",
+      "type": "object",
+      "properties": {
+        "featureSelectionPreference": {
+          "description": "Required. Feature selection preference.",
+          "type": "string",
+          "enumDescriptions": [
+            "Unspecified feature selection preference.",
+            "Prefer higher quality over lower cost.",
+            "Balanced feature selection preference.",
+            "Prefer lower cost over higher quality."
+          ],
+          "enum": [
+            "FEATURE_SELECTION_PREFERENCE_UNSPECIFIED",
+            "PRIORITIZE_QUALITY",
+            "BALANCED",
+            "PRIORITIZE_COST"
+          ]
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1CountTokensResponse": {
+      "id": "GoogleCloudAiplatformV1beta1CountTokensResponse",
+      "description": "Response message for PredictionService.CountTokens.",
+      "type": "object",
+      "properties": {
+        "totalTokens": {
+          "description": "The total number of tokens counted across all instances from the request.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "totalBillableCharacters": {
+          "description": "The total number of billable characters counted across all instances from the request.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "promptTokensDetails": {
+          "description": "Output only. List of modalities that were processed in the request input.",
+          "readOnly": true,
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1ModalityTokenCount"
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1ModalityTokenCount": {
+      "id": "GoogleCloudAiplatformV1beta1ModalityTokenCount",
+      "description": "Represents token counting info for a single modality.",
+      "type": "object",
+      "properties": {
+        "modality": {
+          "description": "The modality associated with this token count.",
+          "type": "string",
+          "enumDescriptions": [
+            "Unspecified modality.",
+            "Plain text.",
+            "Image.",
+            "Video.",
+            "Audio.",
+            "Document, e.g. PDF."
+          ],
+          "enum": [
+            "MODALITY_UNSPECIFIED",
+            "TEXT",
+            "IMAGE",
+            "VIDEO",
+            "AUDIO",
+            "DOCUMENT"
+          ]
+        },
+        "tokenCount": {
+          "description": "Number of tokens.",
+          "type": "integer",
+          "format": "int32"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GenerateContentRequest": {
+      "id": "GoogleCloudAiplatformV1beta1GenerateContentRequest",
+      "description": "Request message for [PredictionService.GenerateContent].",
+      "type": "object",
+      "properties": {
+        "contents": {
+          "description": "Required. The content of the current conversation with the model. For single-turn queries, this is a single instance. For multi-turn queries, this is a repeated field that contains conversation history + latest request.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1Content"
+          }
+        },
+        "systemInstruction": {
+          "description": "Optional. The user provided system instructions for the model. Note: only text should be used in parts and content in each part will be in a separate paragraph.",
+          "$ref": "GoogleCloudAiplatformV1beta1Content"
+        },
+        "cachedContent": {
+          "description": "Optional. The name of the cached content used as context to serve the prediction. Note: only used in explicit caching, where users can have control over caching (e.g. what content to cache) and enjoy guaranteed cost savings. Format: `projects/{project}/locations/{location}/cachedContents/{cachedContent}`",
+          "type": "string"
+        },
+        "tools": {
+          "description": "Optional. A list of `Tools` the model may use to generate the next response. A `Tool` is a piece of code that enables the system to interact with external systems to perform an action, or set of actions, outside of knowledge and scope of the model.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1Tool"
+          }
+        },
+        "toolConfig": {
+          "description": "Optional. Tool config. This config is shared for all tools provided in the request.",
+          "$ref": "GoogleCloudAiplatformV1beta1ToolConfig"
+        },
+        "labels": {
+          "description": "Optional. The labels with user-defined metadata for the request. It is used for billing and reporting only. Label keys and values can be no longer than 63 characters (Unicode codepoints) and can only contain lowercase letters, numeric characters, underscores, and dashes. International characters are allowed. Label values are optional. Label keys must start with a letter.",
+          "type": "object",
+          "additionalProperties": {
+            "type": "string"
+          }
+        },
+        "safetySettings": {
+          "description": "Optional. Per request settings for blocking unsafe content. Enforced on GenerateContentResponse.candidates.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1SafetySetting"
+          }
+        },
+        "generationConfig": {
+          "description": "Optional. Generation config.",
+          "$ref": "GoogleCloudAiplatformV1beta1GenerationConfig"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1ToolConfig": {
+      "id": "GoogleCloudAiplatformV1beta1ToolConfig",
+      "description": "Tool config. This config is shared for all tools provided in the request.",
+      "type": "object",
+      "properties": {
+        "functionCallingConfig": {
+          "description": "Optional. Function calling config.",
+          "$ref": "GoogleCloudAiplatformV1beta1FunctionCallingConfig"
+        },
+        "retrievalConfig": {
+          "description": "Optional. Retrieval config.",
+          "$ref": "GoogleCloudAiplatformV1beta1RetrievalConfig"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1FunctionCallingConfig": {
+      "id": "GoogleCloudAiplatformV1beta1FunctionCallingConfig",
+      "description": "Function calling config.",
+      "type": "object",
+      "properties": {
+        "mode": {
+          "description": "Optional. Function calling mode.",
+          "type": "string",
+          "enumDescriptions": [
+            "Unspecified function calling mode. This value should not be used.",
+            "Default model behavior, model decides to predict either function calls or natural language response.",
+            "Model is constrained to always predicting function calls only. If \"allowed_function_names\" are set, the predicted function calls will be limited to any one of \"allowed_function_names\", else the predicted function calls will be any one of the provided \"function_declarations\".",
+            "Model will not predict any function calls. Model behavior is same as when not passing any function declarations."
+          ],
+          "enum": [
+            "MODE_UNSPECIFIED",
+            "AUTO",
+            "ANY",
+            "NONE"
+          ]
+        },
+        "allowedFunctionNames": {
+          "description": "Optional. Function names to call. Only set when the Mode is ANY. Function names should match [FunctionDeclaration.name]. With mode set to ANY, model will predict a function call from the set of function names provided.",
+          "type": "array",
+          "items": {
+            "type": "string"
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RetrievalConfig": {
+      "id": "GoogleCloudAiplatformV1beta1RetrievalConfig",
+      "description": "Retrieval config.",
+      "type": "object",
+      "properties": {
+        "latLng": {
+          "description": "The location of the user.",
+          "$ref": "LatLng"
+        },
+        "languageCode": {
+          "description": "The language code of the user.",
+          "type": "string"
+        }
+      }
+    },
+    "LatLng": {
+      "id": "LatLng",
+      "description": "An object that represents a latitude/longitude pair. This is expressed as a pair of doubles to represent degrees latitude and degrees longitude. Unless specified otherwise, this object must conform to the WGS84 standard. Values must be within normalized ranges.",
+      "type": "object",
+      "properties": {
+        "latitude": {
+          "description": "The latitude in degrees. It must be in the range [-90.0, +90.0].",
+          "type": "number",
+          "format": "double"
+        },
+        "longitude": {
+          "description": "The longitude in degrees. It must be in the range [-180.0, +180.0].",
+          "type": "number",
+          "format": "double"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1SafetySetting": {
+      "id": "GoogleCloudAiplatformV1beta1SafetySetting",
+      "description": "Safety settings.",
+      "type": "object",
+      "properties": {
+        "category": {
+          "description": "Required. Harm category.",
+          "type": "string",
+          "enumDescriptions": [
+            "The harm category is unspecified.",
+            "The harm category is hate speech.",
+            "The harm category is dangerous content.",
+            "The harm category is harassment.",
+            "The harm category is sexually explicit content.",
+            "Deprecated: Election filter is not longer supported. The harm category is civic integrity."
+          ],
+          "enumDeprecated": [
+            false,
+            false,
+            false,
+            false,
+            false,
+            true
+          ],
+          "enum": [
+            "HARM_CATEGORY_UNSPECIFIED",
+            "HARM_CATEGORY_HATE_SPEECH",
+            "HARM_CATEGORY_DANGEROUS_CONTENT",
+            "HARM_CATEGORY_HARASSMENT",
+            "HARM_CATEGORY_SEXUALLY_EXPLICIT",
+            "HARM_CATEGORY_CIVIC_INTEGRITY"
+          ]
+        },
+        "threshold": {
+          "description": "Required. The harm block threshold.",
+          "type": "string",
+          "enumDescriptions": [
+            "Unspecified harm block threshold.",
+            "Block low threshold and above (i.e. block more).",
+            "Block medium threshold and above.",
+            "Block only high threshold (i.e. block less).",
+            "Block none.",
+            "Turn off the safety filter."
+          ],
+          "enum": [
+            "HARM_BLOCK_THRESHOLD_UNSPECIFIED",
+            "BLOCK_LOW_AND_ABOVE",
+            "BLOCK_MEDIUM_AND_ABOVE",
+            "BLOCK_ONLY_HIGH",
+            "BLOCK_NONE",
+            "OFF"
+          ]
+        },
+        "method": {
+          "description": "Optional. Specify if the threshold is used for probability or severity score. If not specified, the threshold is used for probability score.",
+          "type": "string",
+          "enumDescriptions": [
+            "The harm block method is unspecified.",
+            "The harm block method uses both probability and severity scores.",
+            "The harm block method uses the probability score."
+          ],
+          "enum": [
+            "HARM_BLOCK_METHOD_UNSPECIFIED",
+            "SEVERITY",
+            "PROBABILITY"
+          ]
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GenerateContentResponse": {
+      "id": "GoogleCloudAiplatformV1beta1GenerateContentResponse",
+      "description": "Response message for [PredictionService.GenerateContent].",
+      "type": "object",
+      "properties": {
+        "candidates": {
+          "description": "Output only. Generated candidates.",
+          "readOnly": true,
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1Candidate"
+          }
+        },
+        "modelVersion": {
+          "description": "Output only. The model version used to generate the response.",
+          "readOnly": true,
+          "type": "string"
+        },
+        "createTime": {
+          "description": "Output only. Timestamp when the request is made to the server.",
+          "readOnly": true,
+          "type": "string",
+          "format": "google-datetime"
+        },
+        "responseId": {
+          "description": "Output only. response_id is used to identify each response. It is the encoding of the event_id.",
+          "readOnly": true,
+          "type": "string"
+        },
+        "promptFeedback": {
+          "description": "Output only. Content filter results for a prompt sent in the request. Note: Sent only in the first stream chunk. Only happens when no candidates were generated due to content violations.",
+          "readOnly": true,
+          "$ref": "GoogleCloudAiplatformV1beta1GenerateContentResponsePromptFeedback"
+        },
+        "usageMetadata": {
+          "description": "Usage metadata about the response(s).",
+          "$ref": "GoogleCloudAiplatformV1beta1GenerateContentResponseUsageMetadata"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1Candidate": {
+      "id": "GoogleCloudAiplatformV1beta1Candidate",
+      "description": "A response candidate generated from the model.",
+      "type": "object",
+      "properties": {
+        "index": {
+          "description": "Output only. Index of the candidate.",
+          "readOnly": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "content": {
+          "description": "Output only. Content parts of the candidate.",
+          "readOnly": true,
+          "$ref": "GoogleCloudAiplatformV1beta1Content"
+        },
+        "avgLogprobs": {
+          "description": "Output only. Average log probability score of the candidate.",
+          "readOnly": true,
+          "type": "number",
+          "format": "double"
+        },
+        "logprobsResult": {
+          "description": "Output only. Log-likelihood scores for the response tokens and top tokens",
+          "readOnly": true,
+          "$ref": "GoogleCloudAiplatformV1beta1LogprobsResult"
+        },
+        "finishReason": {
+          "description": "Output only. The reason why the model stopped generating tokens. If empty, the model has not stopped generating the tokens.",
+          "readOnly": true,
+          "type": "string",
+          "enumDescriptions": [
+            "The finish reason is unspecified.",
+            "Token generation reached a natural stopping point or a configured stop sequence.",
+            "Token generation reached the configured maximum output tokens.",
+            "Token generation stopped because the content potentially contains safety violations. NOTE: When streaming, content is empty if content filters blocks the output.",
+            "The token generation stopped because of potential recitation.",
+            "All other reasons that stopped the token generation.",
+            "Token generation stopped because the content contains forbidden terms.",
+            "Token generation stopped for potentially containing prohibited content.",
+            "Token generation stopped because the content potentially contains Sensitive Personally Identifiable Information (SPII).",
+            "The function call generated by the model is invalid."
+          ],
+          "enum": [
+            "FINISH_REASON_UNSPECIFIED",
+            "STOP",
+            "MAX_TOKENS",
+            "SAFETY",
+            "RECITATION",
+            "OTHER",
+            "BLOCKLIST",
+            "PROHIBITED_CONTENT",
+            "SPII",
+            "MALFORMED_FUNCTION_CALL"
+          ]
+        },
+        "safetyRatings": {
+          "description": "Output only. List of ratings for the safety of a response candidate. There is at most one rating per category.",
+          "readOnly": true,
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1SafetyRating"
+          }
+        },
+        "finishMessage": {
+          "description": "Output only. Describes the reason the mode stopped generating tokens in more detail. This is only filled when `finish_reason` is set.",
+          "readOnly": true,
+          "type": "string"
+        },
+        "citationMetadata": {
+          "description": "Output only. Source attribution of the generated content.",
+          "readOnly": true,
+          "$ref": "GoogleCloudAiplatformV1beta1CitationMetadata"
+        },
+        "groundingMetadata": {
+          "description": "Output only. Metadata specifies sources used to ground generated content.",
+          "readOnly": true,
+          "$ref": "GoogleCloudAiplatformV1beta1GroundingMetadata"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1LogprobsResult": {
+      "id": "GoogleCloudAiplatformV1beta1LogprobsResult",
+      "description": "Logprobs Result",
+      "type": "object",
+      "properties": {
+        "topCandidates": {
+          "description": "Length = total number of decoding steps.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1LogprobsResultTopCandidates"
+          }
+        },
+        "chosenCandidates": {
+          "description": "Length = total number of decoding steps. The chosen candidates may or may not be in top_candidates.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1LogprobsResultCandidate"
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1LogprobsResultTopCandidates": {
+      "id": "GoogleCloudAiplatformV1beta1LogprobsResultTopCandidates",
+      "description": "Candidates with top log probabilities at each decoding step.",
+      "type": "object",
+      "properties": {
+        "candidates": {
+          "description": "Sorted by log probability in descending order.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1LogprobsResultCandidate"
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1LogprobsResultCandidate": {
+      "id": "GoogleCloudAiplatformV1beta1LogprobsResultCandidate",
+      "description": "Candidate for the logprobs token and score.",
+      "type": "object",
+      "properties": {
+        "token": {
+          "description": "The candidate's token string value.",
+          "type": "string"
+        },
+        "tokenId": {
+          "description": "The candidate's token id value.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "logProbability": {
+          "description": "The candidate's log probability.",
+          "type": "number",
+          "format": "float"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1SafetyRating": {
+      "id": "GoogleCloudAiplatformV1beta1SafetyRating",
+      "description": "Safety rating corresponding to the generated content.",
+      "type": "object",
+      "properties": {
+        "category": {
+          "description": "Output only. Harm category.",
+          "readOnly": true,
+          "type": "string",
+          "enumDescriptions": [
+            "The harm category is unspecified.",
+            "The harm category is hate speech.",
+            "The harm category is dangerous content.",
+            "The harm category is harassment.",
+            "The harm category is sexually explicit content.",
+            "Deprecated: Election filter is not longer supported. The harm category is civic integrity."
+          ],
+          "enumDeprecated": [
+            false,
+            false,
+            false,
+            false,
+            false,
+            true
+          ],
+          "enum": [
+            "HARM_CATEGORY_UNSPECIFIED",
+            "HARM_CATEGORY_HATE_SPEECH",
+            "HARM_CATEGORY_DANGEROUS_CONTENT",
+            "HARM_CATEGORY_HARASSMENT",
+            "HARM_CATEGORY_SEXUALLY_EXPLICIT",
+            "HARM_CATEGORY_CIVIC_INTEGRITY"
+          ]
+        },
+        "probability": {
+          "description": "Output only. Harm probability levels in the content.",
+          "readOnly": true,
+          "type": "string",
+          "enumDescriptions": [
+            "Harm probability unspecified.",
+            "Negligible level of harm.",
+            "Low level of harm.",
+            "Medium level of harm.",
+            "High level of harm."
+          ],
+          "enum": [
+            "HARM_PROBABILITY_UNSPECIFIED",
+            "NEGLIGIBLE",
+            "LOW",
+            "MEDIUM",
+            "HIGH"
+          ]
+        },
+        "probabilityScore": {
+          "description": "Output only. Harm probability score.",
+          "readOnly": true,
+          "type": "number",
+          "format": "float"
+        },
+        "severity": {
+          "description": "Output only. Harm severity levels in the content.",
+          "readOnly": true,
+          "type": "string",
+          "enumDescriptions": [
+            "Harm severity unspecified.",
+            "Negligible level of harm severity.",
+            "Low level of harm severity.",
+            "Medium level of harm severity.",
+            "High level of harm severity."
+          ],
+          "enum": [
+            "HARM_SEVERITY_UNSPECIFIED",
+            "HARM_SEVERITY_NEGLIGIBLE",
+            "HARM_SEVERITY_LOW",
+            "HARM_SEVERITY_MEDIUM",
+            "HARM_SEVERITY_HIGH"
+          ]
+        },
+        "severityScore": {
+          "description": "Output only. Harm severity score.",
+          "readOnly": true,
+          "type": "number",
+          "format": "float"
+        },
+        "blocked": {
+          "description": "Output only. Indicates whether the content was filtered out because of this rating.",
+          "readOnly": true,
+          "type": "boolean"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1CitationMetadata": {
+      "id": "GoogleCloudAiplatformV1beta1CitationMetadata",
+      "description": "A collection of source attributions for a piece of content.",
+      "type": "object",
+      "properties": {
+        "citations": {
+          "description": "Output only. List of citations.",
+          "readOnly": true,
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1Citation"
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1Citation": {
+      "id": "GoogleCloudAiplatformV1beta1Citation",
+      "description": "Source attributions for content.",
+      "type": "object",
+      "properties": {
+        "startIndex": {
+          "description": "Output only. Start index into the content.",
+          "readOnly": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "endIndex": {
+          "description": "Output only. End index into the content.",
+          "readOnly": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "uri": {
+          "description": "Output only. Url reference of the attribution.",
+          "readOnly": true,
+          "type": "string"
+        },
+        "title": {
+          "description": "Output only. Title of the attribution.",
+          "readOnly": true,
+          "type": "string"
+        },
+        "license": {
+          "description": "Output only. License of the attribution.",
+          "readOnly": true,
+          "type": "string"
+        },
+        "publicationDate": {
+          "description": "Output only. Publication date of the attribution.",
+          "readOnly": true,
+          "$ref": "Date"
+        }
+      }
+    },
+    "Date": {
+      "id": "Date",
+      "description": "Represents a whole or partial calendar date, such as a birthday. The time of day and time zone are either specified elsewhere or are insignificant. The date is relative to the Gregorian Calendar. This can represent one of the following: * A full date, with non-zero year, month, and day values. * A month and day, with a zero year (for example, an anniversary). * A year on its own, with a zero month and a zero day. * A year and month, with a zero day (for example, a credit card expiration date). Related types: * google.type.TimeOfDay * google.type.DateTime * google.protobuf.Timestamp",
+      "type": "object",
+      "properties": {
+        "year": {
+          "description": "Year of the date. Must be from 1 to 9999, or 0 to specify a date without a year.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "month": {
+          "description": "Month of a year. Must be from 1 to 12, or 0 to specify a year without a month and day.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "day": {
+          "description": "Day of a month. Must be from 1 to 31 and valid for the year and month, or 0 to specify a year by itself or a year and month where the day isn't significant.",
+          "type": "integer",
+          "format": "int32"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GroundingMetadata": {
+      "id": "GoogleCloudAiplatformV1beta1GroundingMetadata",
+      "description": "Metadata returned to client when grounding is enabled.",
+      "type": "object",
+      "properties": {
+        "webSearchQueries": {
+          "description": "Optional. Web search queries for the following-up web search.",
+          "type": "array",
+          "items": {
+            "type": "string"
+          }
+        },
+        "searchEntryPoint": {
+          "description": "Optional. Google search entry for the following-up web searches.",
+          "$ref": "GoogleCloudAiplatformV1beta1SearchEntryPoint"
+        },
+        "retrievalQueries": {
+          "description": "Optional. Queries executed by the retrieval tools.",
+          "type": "array",
+          "items": {
+            "type": "string"
+          }
+        },
+        "groundingChunks": {
+          "description": "List of supporting references retrieved from specified grounding source.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1GroundingChunk"
+          }
+        },
+        "groundingSupports": {
+          "description": "Optional. List of grounding support.",
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1GroundingSupport"
+          }
+        },
+        "retrievalMetadata": {
+          "description": "Optional. Output only. Retrieval metadata.",
+          "readOnly": true,
+          "$ref": "GoogleCloudAiplatformV1beta1RetrievalMetadata"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1SearchEntryPoint": {
+      "id": "GoogleCloudAiplatformV1beta1SearchEntryPoint",
+      "description": "Google search entry point.",
+      "type": "object",
+      "properties": {
+        "renderedContent": {
+          "description": "Optional. Web content snippet that can be embedded in a web page or an app webview.",
+          "type": "string"
+        },
+        "sdkBlob": {
+          "description": "Optional. Base64 encoded JSON representing array of tuple.",
+          "type": "string",
+          "format": "byte"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GroundingChunk": {
+      "id": "GoogleCloudAiplatformV1beta1GroundingChunk",
+      "description": "Grounding chunk.",
+      "type": "object",
+      "properties": {
+        "web": {
+          "description": "Grounding chunk from the web.",
+          "$ref": "GoogleCloudAiplatformV1beta1GroundingChunkWeb"
+        },
+        "retrievedContext": {
+          "description": "Grounding chunk from context retrieved by the retrieval tools.",
+          "$ref": "GoogleCloudAiplatformV1beta1GroundingChunkRetrievedContext"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GroundingChunkWeb": {
+      "id": "GoogleCloudAiplatformV1beta1GroundingChunkWeb",
+      "description": "Chunk from the web.",
+      "type": "object",
+      "properties": {
+        "uri": {
+          "description": "URI reference of the chunk.",
+          "type": "string"
+        },
+        "title": {
+          "description": "Title of the chunk.",
+          "type": "string"
+        },
+        "domain": {
+          "description": "Domain of the (original) URI.",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GroundingChunkRetrievedContext": {
+      "id": "GoogleCloudAiplatformV1beta1GroundingChunkRetrievedContext",
+      "description": "Chunk from context retrieved by the retrieval tools.",
+      "type": "object",
+      "properties": {
+        "ragChunk": {
+          "description": "Additional context for the RAG retrieval result. This is only populated when using the RAG retrieval tool.",
+          "$ref": "GoogleCloudAiplatformV1beta1RagChunk"
+        },
+        "uri": {
+          "description": "URI reference of the attribution.",
+          "type": "string"
+        },
+        "title": {
+          "description": "Title of the attribution.",
+          "type": "string"
+        },
+        "text": {
+          "description": "Text of the attribution.",
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RagChunk": {
+      "id": "GoogleCloudAiplatformV1beta1RagChunk",
+      "description": "A RagChunk includes the content of a chunk of a RagFile, and associated metadata.",
+      "type": "object",
+      "properties": {
+        "text": {
+          "description": "The content of the chunk.",
+          "type": "string"
+        },
+        "pageSpan": {
+          "description": "If populated, represents where the chunk starts and ends in the document.",
+          "$ref": "GoogleCloudAiplatformV1beta1RagChunkPageSpan"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RagChunkPageSpan": {
+      "id": "GoogleCloudAiplatformV1beta1RagChunkPageSpan",
+      "description": "Represents where the chunk starts and ends in the document.",
+      "type": "object",
+      "properties": {
+        "firstPage": {
+          "description": "Page where chunk starts in the document. Inclusive. 1-indexed.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "lastPage": {
+          "description": "Page where chunk ends in the document. Inclusive. 1-indexed.",
+          "type": "integer",
+          "format": "int32"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GroundingSupport": {
+      "id": "GoogleCloudAiplatformV1beta1GroundingSupport",
+      "description": "Grounding support.",
+      "type": "object",
+      "properties": {
+        "segment": {
+          "description": "Segment of the content this support belongs to.",
+          "$ref": "GoogleCloudAiplatformV1beta1Segment"
+        },
+        "groundingChunkIndices": {
+          "description": "A list of indices (into 'grounding_chunk') specifying the citations associated with the claim. For instance [1,3,4] means that grounding_chunk[1], grounding_chunk[3], grounding_chunk[4] are the retrieved content attributed to the claim.",
+          "type": "array",
+          "items": {
+            "type": "integer",
+            "format": "int32"
+          }
+        },
+        "confidenceScores": {
+          "description": "Confidence score of the support references. Ranges from 0 to 1. 1 is the most confident. This list must have the same size as the grounding_chunk_indices.",
+          "type": "array",
+          "items": {
+            "type": "number",
+            "format": "float"
+          }
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1Segment": {
+      "id": "GoogleCloudAiplatformV1beta1Segment",
+      "description": "Segment of the content.",
+      "type": "object",
+      "properties": {
+        "partIndex": {
+          "description": "Output only. The index of a Part object within its parent Content object.",
+          "readOnly": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "startIndex": {
+          "description": "Output only. Start index in the given Part, measured in bytes. Offset from the start of the Part, inclusive, starting at zero.",
+          "readOnly": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "endIndex": {
+          "description": "Output only. End index in the given Part, measured in bytes. Offset from the start of the Part, exclusive, starting at zero.",
+          "readOnly": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "text": {
+          "description": "Output only. The text corresponding to the segment from the response.",
+          "readOnly": true,
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1RetrievalMetadata": {
+      "id": "GoogleCloudAiplatformV1beta1RetrievalMetadata",
+      "description": "Metadata related to retrieval in the grounding flow.",
+      "type": "object",
+      "properties": {
+        "googleSearchDynamicRetrievalScore": {
+          "description": "Optional. Score indicating how likely information from Google Search could help answer the prompt. The score is in the range `[0, 1]`, where 0 is the least likely and 1 is the most likely. This score is only populated when Google Search grounding and dynamic retrieval is enabled. It will be compared to the threshold to determine whether to trigger Google Search.",
+          "type": "number",
+          "format": "float"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GenerateContentResponsePromptFeedback": {
+      "id": "GoogleCloudAiplatformV1beta1GenerateContentResponsePromptFeedback",
+      "description": "Content filter results for a prompt sent in the request.",
+      "type": "object",
+      "properties": {
+        "blockReason": {
+          "description": "Output only. Blocked reason.",
+          "readOnly": true,
+          "type": "string",
+          "enumDescriptions": [
+            "Unspecified blocked reason.",
+            "Candidates blocked due to safety.",
+            "Candidates blocked due to other reason.",
+            "Candidates blocked due to the terms which are included from the terminology blocklist.",
+            "Candidates blocked due to prohibited content."
+          ],
+          "enum": [
+            "BLOCKED_REASON_UNSPECIFIED",
+            "SAFETY",
+            "OTHER",
+            "BLOCKLIST",
+            "PROHIBITED_CONTENT"
+          ]
+        },
+        "safetyRatings": {
+          "description": "Output only. Safety ratings.",
+          "readOnly": true,
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1SafetyRating"
+          }
+        },
+        "blockReasonMessage": {
+          "description": "Output only. A readable block reason message.",
+          "readOnly": true,
+          "type": "string"
+        }
+      }
+    },
+    "GoogleCloudAiplatformV1beta1GenerateContentResponseUsageMetadata": {
+      "id": "GoogleCloudAiplatformV1beta1GenerateContentResponseUsageMetadata",
+      "description": "Usage metadata about response(s).",
+      "type": "object",
+      "properties": {
+        "promptTokenCount": {
+          "description": "Number of tokens in the request. When `cached_content` is set, this is still the total effective prompt size meaning this includes the number of tokens in the cached content.",
+          "type": "integer",
+          "format": "int32"
+        },
+        "candidatesTokenCount": {
+          "description": "Number of tokens in the response(s).",
+          "type": "integer",
+          "format": "int32"
+        },
+        "toolUsePromptTokenCount": {
+          "description": "Output only. Number of tokens present in tool-use prompt(s).",
+          "readOnly": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "thoughtsTokenCount": {
+          "description": "Output only. Number of tokens present in thoughts output.",
+          "readOnly": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "totalTokenCount": {
+          "description": "Total token count for prompt, response candidates, and tool-use prompts (if present).",
+          "type": "integer",
+          "format": "int32"
+        },
+        "cachedContentTokenCount": {
+          "description": "Output only. Number of tokens in the cached part in the input (the cached content).",
+          "readOnly": true,
+          "type": "integer",
+          "format": "int32"
+        },
+        "promptTokensDetails": {
+          "description": "Output only. List of modalities that were processed in the request input.",
+          "readOnly": true,
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1ModalityTokenCount"
+          }
+        },
+        "cacheTokensDetails": {
+          "description": "Output only. List of modalities of the cached content in the request input.",
+          "readOnly": true,
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1ModalityTokenCount"
+          }
+        },
+        "candidatesTokensDetails": {
+          "description": "Output only. List of modalities that were returned in the response.",
+          "readOnly": true,
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1ModalityTokenCount"
+          }
+        },
+        "toolUsePromptTokensDetails": {
+          "description": "Output only. List of modalities that were processed for tool-use request inputs.",
+          "readOnly": true,
+          "type": "array",
+          "items": {
+            "$ref": "GoogleCloudAiplatformV1beta1ModalityTokenCount"
+          }
+        },
+        "trafficType": {
+          "description": "Output only. Traffic type. This shows whether a request consumes Pay-As-You-Go or Provisioned Throughput quota.",
+          "readOnly": true,
+          "type": "string",
+          "enumDescriptions": [
+            "Unspecified request traffic type.",
+            "Type for Pay-As-You-Go traffic.",
+            "Type for Provisioned Throughput traffic."
+          ],
+          "enum": [
+            "TRAFFIC_TYPE_UNSPECIFIED",
+            "ON_DEMAND",
+            "PROVISIONED_THROUGHPUT"
+          ]
+        }
+      }
+    }
+  },
+  "parameters": {
+    "access_token": {
+      "type": "string",
+      "description": "OAuth access token.",
+      "location": "query"
+    },
+    "alt": {
+      "type": "string",
+      "description": "Data format for response.",
+      "default": "json",
+      "enum": [
+        "json",
+        "media",
+        "proto"
+      ],
+      "enumDescriptions": [
+        "Responses with Content-Type of application/json",
+        "Media download with context-dependent Content-Type",
+        "Responses with Content-Type of application/x-protobuf"
+      ],
+      "location": "query"
+    },
+    "callback": {
+      "type": "string",
+      "description": "JSONP",
+      "location": "query"
+    },
+    "fields": {
+      "type": "string",
+      "description": "Selector specifying which fields to include in a partial response.",
+      "location": "query"
+    },
+    "key": {
+      "type": "string",
+      "description": "API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.",
+      "location": "query"
+    },
+    "oauth_token": {
+      "type": "string",
+      "description": "OAuth 2.0 token for the current user.",
+      "location": "query"
+    },
+    "prettyPrint": {
+      "type": "boolean",
+      "description": "Returns response with indentations and line breaks.",
+      "default": "true",
+      "location": "query"
+    },
+    "quotaUser": {
+      "type": "string",
+      "description": "Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.",
+      "location": "query"
+    },
+    "upload_protocol": {
+      "type": "string",
+      "description": "Upload protocol for media (e.g. \"raw\", \"multipart\").",
+      "location": "query"
+    },
+    "uploadType": {
+      "type": "string",
+      "description": "Legacy upload protocol for media (e.g. \"media\", \"multipart\").",
+      "location": "query"
+    },
+    "$.xgafv": {
+      "type": "string",
+      "description": "V1 error format.",
+      "enum": [
+        "1",
+        "2"
+      ],
+      "enumDescriptions": [
+        "v1 error format",
+        "v2 error format"
+      ],
+      "location": "query"
+    }
+  },
+  "documentationLink": "https://firebase.google.com",
+  "ownerDomain": "google.com",
+  "title": "Vertex AI in Firebase API",
+  "id": "firebasevertexai:v1beta",
+  "version": "v1beta",
+  "batchPath": "batch",
+  "fullyEncodeReservedExpansion": true,
+  "revision": "20250416"
+}
```


