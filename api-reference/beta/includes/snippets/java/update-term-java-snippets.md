---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c55dd3e0ba0ebc3e3fdfbefdfd2420e2b4a6f074
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972561"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Term term = new Term();
LinkedList<LocalizedLabel> labelsList = new LinkedList<LocalizedLabel>();
LocalizedLabel labels = new LocalizedLabel();
labels.name = "changedLabel";
labels.languageTag = "en-US";
labels.isDefault = true;
labelsList.add(labels);
term.labels = labelsList;

graphClient.termStore().sets("{setId}").terms("{termId}")
    .buildRequest()
    .patch(term);

```