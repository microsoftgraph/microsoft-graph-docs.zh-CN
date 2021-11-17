---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81bdf5e7dc9e88fdce55979d25de3fbc8a75195a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991548"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

result, err := graphClient.Policies().AdminConsentRequestPolicy().Get(options)


```