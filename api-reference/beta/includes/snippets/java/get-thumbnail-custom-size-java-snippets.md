---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58268d1117443e4965073d8597f7103f20187008
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955794"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("select", "c300x400_Crop"));

IThumbnailSetCollectionPage thumbnails = graphClient.me().drive().items("{item-id}").thumbnails()
    .buildRequest( requestOptions )
    .get();

```