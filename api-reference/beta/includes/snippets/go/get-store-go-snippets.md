---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fb052a6eb3f7ad9622e6449f1c0970901e2bf1c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001664"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
result, err := graphClient.SitesById(&siteId).TermStore().Get(options)


```