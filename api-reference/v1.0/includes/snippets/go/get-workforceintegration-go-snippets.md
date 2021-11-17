---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d80758dc6a6c0efe2055053814d1e6790faba210
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022727"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

workforceIntegrationId := "workforceIntegration-id"
result, err := graphClient.Teamwork().WorkforceIntegrationsById(&workforceIntegrationId).Get(options)


```