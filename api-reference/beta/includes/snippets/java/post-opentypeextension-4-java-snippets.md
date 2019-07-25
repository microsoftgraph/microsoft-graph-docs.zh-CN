---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6f94c85827a11660d9b0df68163b2bb3b67d4628
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878354"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.HTML;
body.content = "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>";
post.body = body;
LinkedList<Extension> extensionsList = new LinkedList<Extension>();
Extension extensions = new Extension();
extensions.additionalDataManager().put("@odata.type", new JsonPrimitive("microsoft.graph.openTypeExtension"));
extensions.extensionName = "Com.Contoso.HR";
extensions.companyName = "Contoso";
extensions.expirationDate = "2015-07-03T13:04:00Z";
LinkedList<String> topPicksList = new LinkedList<String>();
topPicksList.add("Employees only");
topPicksList.add("Add spouse or guest");
topPicksList.add("Add family");
extensions.topPicks = topPicksList;
extensionsList.add(extensions);
post.extensions = extensionsList;

graphClient.groups("37df2ff0-0de0-4c33-8aee-75289364aef6").threads("AAQkADJizZJpEWwqDHsEpV_KA==").posts("AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=")
    .reply(post)
    .buildRequest()
    .post();

```