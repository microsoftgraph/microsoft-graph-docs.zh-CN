---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d01fc924bdc47ad6ad778413c23b6c0e63019ee8
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943592"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] accessReviewScheduleDefinition = Base64.getDecoder().decode("{  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",  "displayName": "Test world UPDATED NAME!",  "descriptionForAdmins": "Test world",  "descriptionForReviewers": "Test world",  "scope": {    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",    "queryType": "MicrosoftGraph"  },  "instanceEnumerationScope": {    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",    "queryType": "MicrosoftGraph"  },  "reviewers": [],  "settings": {    "mailNotificationsEnabled": true,    "reminderNotificationsEnabled": true,    "justificationRequiredOnApproval": true,    "defaultDecisionEnabled": false,    "defaultDecision": "None",    "instanceDurationInDays": 3,    "autoApplyDecisionsEnabled": false,    "recommendationsEnabled": true,    "recurrence": {      "pattern": {        "type": "weekly",        "interval": 1      },      "range": {        "type": "noEnd",        "startDate": "2020-09-15"      }    }  }}");
    graphClient.identityGovernance().accessReviews().definitions("60860cdd-fb4d-4054-91ba-f75e04444aa6")
    .buildRequest()
    .put(accessReviewScheduleDefinition);

```