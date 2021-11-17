---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64a3ad8eb191130bedb9035e095a5b6f6cd149d8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018856"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
result, err := graphClient.SitesById(&siteId).TermStore().Groups().Get(options)


```