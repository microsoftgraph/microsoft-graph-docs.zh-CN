---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd5a9beeaefe2235b3f4ea28c68f9ec2de52cd6dd323f112a9e4214f6018a5c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161397"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonWebsite personWebsite = new PersonWebsite();
personWebsite.description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway";

graphClient.me().profile().websites("{id}")
    .buildRequest()
    .patch(personWebsite);

```