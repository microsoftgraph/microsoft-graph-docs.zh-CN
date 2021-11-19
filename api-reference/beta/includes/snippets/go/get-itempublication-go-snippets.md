---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20c3c8d95408f3a1d8594ac61fd1f7bc084bfb38
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102748"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemPublicationId := "itemPublication-id"
result, err := graphClient.Me().Profile().PublicationsById(&itemPublicationId).Get(options)


```