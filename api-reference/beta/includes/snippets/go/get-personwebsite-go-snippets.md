---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cc7fefe58bd90d75c02917810232776c3bc5e92
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099278"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personWebsiteId := "personWebsite-id"
result, err := graphClient.Me().Profile().WebsitesById(&personWebsiteId).Get(options)


```