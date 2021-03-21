---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5462c4af00ca8312775a4667dd1316cbbece52ff
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969541"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroupCollectionPage sectionGroups = graphClient.me().onenote().sectionGroups()
    .buildRequest()
    .get();

```