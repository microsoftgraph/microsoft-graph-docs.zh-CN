---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8c9413b33e9a777d832b0b2bc4d728fcbb9cc57
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083431"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Admin().Windows().Updates().Deployments().Get(options)


```