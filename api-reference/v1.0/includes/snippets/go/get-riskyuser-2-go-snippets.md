---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88474aee7612bb7d7e15c2a30a739a359ae6c017
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134354"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.IdentityProtection().RiskyUsers().Get(nil)


```