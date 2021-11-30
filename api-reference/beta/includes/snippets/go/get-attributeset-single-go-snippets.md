---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 000379010042ed5dec4c4f134c6c6ca40e8c96ac
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223619"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

attributeSetId := "attributeSet-id"
result, err := graphClient.Directory().AttributeSetsById(&attributeSetId).Get(options)


```