---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be42dbb962550fb98d4291b98a8cff3ebf0f13233e54e487be0cfa4efef04e13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219040"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProfilePhotoCollectionPage photos = graphClient.groups("{id}").photos()
    .buildRequest()
    .get();

```