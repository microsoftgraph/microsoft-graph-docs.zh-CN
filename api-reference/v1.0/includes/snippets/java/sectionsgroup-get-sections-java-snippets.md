---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5122d1ba379ef21396c8f065acfc2461879799a76b79ae5ab6fc854e27fbd82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220386"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSectionCollectionPage sections = graphClient.me().onenote().sectionGroups("{id}").sections()
    .buildRequest()
    .get();

```