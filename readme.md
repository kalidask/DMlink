# RED HAT DECISION MANAGER 7 - A Simple DMN Project to Validate Data Fields

## Status: In-Progress
Request :
{
  "model-namespace" : "https://github.com/kiegroup/drools/kie-dmn/_B22F98AA-0976-459E-84B2-BCB719C2EA11",
  "model-name" : "validateDta",
  "decision-name" : [ ],
  "decision-id" : [ ],
  "dmn-context" : 
{
"firstName" : "Shivnagi",
"lastName":"23",
"abn":"123",
"mobileNumber":"1987t34568",
"birthDate":"2021-12-12", 
"loanData":
{
	"loanStatus":"N",
	"loanValue": "123"
}
}
}

Response:
{
  "type": "SUCCESS",
  "msg": "OK from container 'dmnValidation_1.0.0-SNAPSHOT'",
  "result": {
    "dmn-evaluation-result": {
      "messages": [],
      "model-namespace": "https://github.com/kiegroup/drools/kie-dmn/_B22F98AA-0976-459E-84B2-BCB719C2EA11",
      "model-name": "validateDta",
      "decision-name": [],
      "dmn-context": {
        "lastName": "23",
        "firstNameValidated": true,
        "fieldValidation": false,
        "mobileNumber": "1987t34568",
        "birthDateFormatValidation": "Date Format incorrect",
        "dependentField": "Record ok",
        "abn": "123",
        "birthDate": "2021-12-12",
        "lastNameValidated": false,
        "firstName": "Shivnagi",
        "mobileValidation": false,
        "abnValidated": false,
        "loanData": {
          "loanStatus": "N",
          "loanValue": "123"
        }
      },
      "decision-results": {
        "_D1CD4FB0-4BC6-43CB-A845-76D37B33F43D": {
          "messages": [],
          "decision-id": "_D1CD4FB0-4BC6-43CB-A845-76D37B33F43D",
          "decision-name": "lastNameValidated",
          "result": false,
          "status": "SUCCEEDED"
        },
        "_3FA392EA-A627-4C89-84C3-6C3F5AC17FDF": {
          "messages": [],
          "decision-id": "_3FA392EA-A627-4C89-84C3-6C3F5AC17FDF",
          "decision-name": "dependentField",
          "result": "Record ok",
          "status": "SUCCEEDED"
        },
        "_7F55E982-F2AD-4D1F-A0E3-C0FF90A2CB78": {
          "messages": [],
          "decision-id": "_7F55E982-F2AD-4D1F-A0E3-C0FF90A2CB78",
          "decision-name": "mobileValidation",
          "result": false,
          "status": "SUCCEEDED"
        },
        "_E57A87CD-AC3C-485D-BADB-9B74441AA2F0": {
          "messages": [],
          "decision-id": "_E57A87CD-AC3C-485D-BADB-9B74441AA2F0",
          "decision-name": "birthDateFormatValidation",
          "result": "Date Format incorrect",
          "status": "SUCCEEDED"
        },
        "_F5C17A30-3698-4BAF-A0C3-2426C6263ECC": {
          "messages": [],
          "decision-id": "_F5C17A30-3698-4BAF-A0C3-2426C6263ECC",
          "decision-name": "fieldValidation",
          "result": false,
          "status": "SUCCEEDED"
        },
        "_F159061B-0CEB-462C-8DBD-84DBD41B1B10": {
          "messages": [],
          "decision-id": "_F159061B-0CEB-462C-8DBD-84DBD41B1B10",
          "decision-name": "firstNameValidated",
          "result": true,
          "status": "SUCCEEDED"
        },
        "_B94EEB70-86B1-4A79-9D72-8E01F4DB4A83": {
          "messages": [],
          "decision-id": "_B94EEB70-86B1-4A79-9D72-8E01F4DB4A83",
          "decision-name": "abnValidated",
          "result": false,
          "status": "SUCCEEDED"
        }
      }
    }
  }
}

