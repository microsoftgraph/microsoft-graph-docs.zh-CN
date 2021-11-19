---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66993905a9810b869cf2607ecc14bdb04717d3d7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093140"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

workforceIntegrationId := "workforceIntegration-id"
result, err := graphClient.Teamwork().WorkforceIntegrationsById(&workforceIntegrationId).Get(options)


```