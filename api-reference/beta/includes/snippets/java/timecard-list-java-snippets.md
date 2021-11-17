---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2c69372002aad90988ee8b0fdb0d7d6ee47ca96ae81f64e69eb973e8e78dba2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274125"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeCardCollectionPage timeCards = graphClient.teams("fd15cad8-80f6-484f-9666-3caf695fbf32").schedule().timeCards()
    .buildRequest()
    .filter("state eq 'clockedOut'")
    .top(2)
    .get();

```