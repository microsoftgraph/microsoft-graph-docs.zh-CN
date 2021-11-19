---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b41791db5b725b0401d3cbe0cbc024c4cb2d52c4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092729"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

orgContactId := "orgContact-id"
graphClient.ContactsById(&orgContactId).Delete(options)


```