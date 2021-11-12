---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ee95027a657da38deb910dc36cbaa35aa3c42963f9dfbb9bd3bec90727f19ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277783"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationThreadCollectionPage threads = graphClient.groups("{id}").threads()
    .buildRequest()
    .get();

```