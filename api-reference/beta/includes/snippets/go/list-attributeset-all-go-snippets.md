---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dbcfa1be9dd06c6a348d755dcba04d6ab2100ea
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225508"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Directory().AttributeSets().Get(options)


```