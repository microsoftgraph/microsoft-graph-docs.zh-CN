---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80caed7e60dad24d4354b9700044db90097879fb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968959"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LanguageProficiencyCollectionPage languages = graphClient.me().profile().languages()
    .buildRequest()
    .get();

```