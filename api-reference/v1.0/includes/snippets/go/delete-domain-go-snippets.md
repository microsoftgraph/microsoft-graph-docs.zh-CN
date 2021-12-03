---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57e1f7f1c790e8235367f623db44d273914fad69
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288573"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

domainId := "domain-id"
graphClient.DomainsById(&domainId).Delete(nil)


```