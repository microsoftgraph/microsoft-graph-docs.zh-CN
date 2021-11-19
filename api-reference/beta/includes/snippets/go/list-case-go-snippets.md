---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 070b0fedb3127c7756da0c10438f8aae6748062e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090075"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Compliance().Ediscovery().Cases().Get(options)


```