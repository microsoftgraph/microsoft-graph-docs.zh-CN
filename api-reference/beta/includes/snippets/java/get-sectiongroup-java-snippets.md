---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2274f4508582b55f53746915a66b5a4f42a798bddc244e113355f46458f8752b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220602"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SectionGroup sectionGroup = graphClient.me().onenote().sectionGroups("{id}")
    .buildRequest()
    .get();

```