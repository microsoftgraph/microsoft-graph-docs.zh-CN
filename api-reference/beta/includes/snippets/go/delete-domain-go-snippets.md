---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1b6183e6069a137e2a59b5b18f10879fb4b28dc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328418"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
graphClient.DomainsById(&domainId).Delete()


```