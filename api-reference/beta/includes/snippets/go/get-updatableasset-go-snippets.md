---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74daf7d1932cca060658037964bae14b736c286a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61004268"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

updatableAssetId := "updatableAsset-id"
result, err := graphClient.Admin().Windows().Updates().UpdatableAssetsById(&updatableAssetId).Get(options)


```