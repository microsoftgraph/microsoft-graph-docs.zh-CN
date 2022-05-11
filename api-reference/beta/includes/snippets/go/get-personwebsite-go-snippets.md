---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0be408a646518c8d176dbe0caf33d6e86f903e3d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327441"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personWebsiteId := "personWebsite-id"
result, err := graphClient.Me().Profile().WebsitesById(&personWebsiteId).Get()


```