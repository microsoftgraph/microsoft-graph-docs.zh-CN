---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31254d546ede305a44420f57197707375c584df5fd7b1068821b223ca6a97663
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219008"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroupCollectionPage sectionGroups = graphClient.me().onenote().sectionGroups()
    .buildRequest()
    .get();

```