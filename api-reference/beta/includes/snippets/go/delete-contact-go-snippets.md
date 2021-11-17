---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c200dbe2345789e94c510a8e2ab804756ba6979
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003308"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

contactId := "contact-id"
graphClient.Me().ContactsById(&contactId).Delete(options)


```