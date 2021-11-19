---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c6c626022f03a0bbe97b8c06c250e755975c4ba
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081725"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

personNameId := "personName-id"
graphClient.Me().Profile().NamesById(&personNameId).Delete(options)


```