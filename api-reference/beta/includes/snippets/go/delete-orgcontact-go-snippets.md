---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdecf1091f5d46d8fc10e55ef1583bf1ad163c5a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002797"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

orgContactId := "orgContact-id"
graphClient.ContactsById(&orgContactId).Delete(options)


```