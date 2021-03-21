---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f801240f69941102da304bb799766a834ebb868
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973688"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageCollectionPage messages = graphClient.me().messages()
    .buildRequest()
    .select("sender,subject")
    .get();

```