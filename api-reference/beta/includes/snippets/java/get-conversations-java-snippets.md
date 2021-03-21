---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5812b0b2da5a50ade7d8d67dff7ac96b0b8d2cdd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973298"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConversationCollectionPage conversations = graphClient.groups("{id}").conversations()
    .buildRequest()
    .get();

```