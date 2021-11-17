---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b696de9b241aaea51adf9b1b40c91f6b89cbe673
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984604"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Lists().Get(options)


```