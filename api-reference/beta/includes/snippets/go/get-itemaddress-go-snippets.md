---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 051b9b5570d8a3c62733e5879e81c406ca080190
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998044"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

itemAddressId := "itemAddress-id"
result, err := graphClient.Me().Profile().AddressesById(&itemAddressId).Get(options)


```