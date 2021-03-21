---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06a448d3ee2be4726227e508e130a3509bc13486
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973197"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonWebsite personWebsite = new PersonWebsite();
personWebsite.description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway";

graphClient.me().profile().websites("{id}")
    .buildRequest()
    .patch(personWebsite);

```