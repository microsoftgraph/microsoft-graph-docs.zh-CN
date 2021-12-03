---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b2143aab9c0e4652bb23ea2c6b6c08f1be759a9
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61288752"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemAddressId := "itemAddress-id"
result, err := graphClient.Me().Profile().AddressesById(&itemAddressId).Get(nil)


```