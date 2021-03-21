---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec2c981c49aaf0b16e67379a30d4bfeaae32379e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978337"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("select", "c300x400_Crop"));

ThumbnailSetCollectionPage thumbnails = graphClient.me().drive().items("{item-id}").thumbnails()
    .buildRequest( requestOptions )
    .get();

```