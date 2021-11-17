---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ade85fcdf00eaa7c5e3f01316ebc72028cea455
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974353"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

contactId := "contact-id"
result, err := graphClient.Me().ContactsById(&contactId).Get(options)


```