---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c07a16a0b3be2168aff2d7456bddfdbc1be2a9d
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287891"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcGalleryImageId := "cloudPcGalleryImage-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().GalleryImagesById(&cloudPcGalleryImageId).Get(nil)


```