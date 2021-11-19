---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5c1d7a4b83c54a32b9ac06a101f2d1c5ddf1d4d5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102749"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemPublicationId := "itemPublication-id"
graphClient.Me().Profile().PublicationsById(&itemPublicationId).Delete(options)


```