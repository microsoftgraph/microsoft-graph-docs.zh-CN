---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba84102c112c3524006c0913534f4cd88442d12b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969459"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSectionCollectionPage sections = graphClient.me().onenote().sectionGroups("{id}").sections()
    .buildRequest()
    .get();

```