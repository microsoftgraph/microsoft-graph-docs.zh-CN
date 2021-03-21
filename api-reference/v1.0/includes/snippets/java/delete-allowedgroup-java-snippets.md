---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a7da9e626c5054632d0fee28b2b4138741578ea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975235"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}").allowedGroups("{groupId}").reference()
    .buildRequest()
    .delete();

```