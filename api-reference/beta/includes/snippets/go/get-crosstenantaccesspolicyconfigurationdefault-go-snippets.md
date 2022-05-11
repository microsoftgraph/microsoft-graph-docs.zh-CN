---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 683d4207d0156bde09b6d3e1819cb3210d6075eb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328301"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.Policies().CrossTenantAccessPolicy().Default().Get()


```