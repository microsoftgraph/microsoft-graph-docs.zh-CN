---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a82ea5934b7ac0c4e8e897943035ac6f5635b7b1
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629809"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Admin().Windows().Updates().UpdatableAssets().Get()


```