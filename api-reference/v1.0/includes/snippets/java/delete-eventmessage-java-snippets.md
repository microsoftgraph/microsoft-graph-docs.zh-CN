---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e3fcd91719ec2facfcdb60269a803f9af5b3cea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984057"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .buildRequest()
    .delete();

```