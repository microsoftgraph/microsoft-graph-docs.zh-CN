---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 212ea8803d71871ba11c8b4c766dbde22bfc56cf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977274"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.applications("{id}").extensionProperties("{id}")
    .buildRequest()
    .delete();

```