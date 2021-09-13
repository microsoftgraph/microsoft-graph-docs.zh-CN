---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d24fbe7485767587aca176e4a37ae362f69f411d430e64ca0d50987255957bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902255"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroupCollectionPage sectionGroups = graphClient.me().onenote().notebooks("{id}").sectionGroups()
    .buildRequest()
    .get();

```