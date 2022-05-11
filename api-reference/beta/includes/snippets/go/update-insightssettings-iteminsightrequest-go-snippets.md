---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 547c93c0dd18652a2a6cfbf8a3e83f7ddbd95d56
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326683"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInsightsSettings()
disabledForGroup := "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
requestBody.SetDisabledForGroup(&disabledForGroup)
organizationId := "organization-id"
graphClient.OrganizationById(&organizationId).Settings().ItemInsights().Patch(requestBody)


```