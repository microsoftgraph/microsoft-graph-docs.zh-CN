---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7cdf8ea4d018afc5c8e901d28bee40a8d66fabe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974978"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] accessReviewScheduleDefinition = Base64.getDecoder().decode("{  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",  "displayName": "Test world UPDATED NAME!",  "descriptionForAdmins": "Test world",  "descriptionForReviewers": "Test world",  "scope": {    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",    "queryType": "MicrosoftGraph"  },  "instanceEnumerationScope": {    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",    "queryType": "MicrosoftGraph"  },  "reviewers": [],  "settings": {    "mailNotificationsEnabled": true,    "reminderNotificationsEnabled": true,    "justificationRequiredOnApproval": true,    "defaultDecisionEnabled": false,    "defaultDecision": "None",    "instanceDurationInDays": 3,    "autoApplyDecisionsEnabled": false,    "recommendationsEnabled": true,    "recurrence": {      "pattern": {        "type": "weekly",        "interval": 1      },      "range": {        "type": "noEnd",        "startDate": "2020-09-15"      }    }  }}");
    graphClient.identityGovernance().accessReviews().definitions("60860cdd-fb4d-4054-91ba-f75e04444aa6")
    .buildRequest()
    .put(accessReviewScheduleDefinition);

```