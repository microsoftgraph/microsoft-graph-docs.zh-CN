---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42ca276f14b04630a187fd608a95fdb7cdff90e8
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096343"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

itemAddressId := "itemAddress-id"
result, err := graphClient.Me().Profile().AddressesById(&itemAddressId).Get(options)


```