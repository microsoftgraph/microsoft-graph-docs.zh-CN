---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a103e7aac95e3614c11e8e97b1fa6ebc56154a99
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089489"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

contactId := "contact-id"
result, err := graphClient.Me().ContactsById(&contactId).Get(options)


```