---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ef0059def9c6873d3bc9c44f4b3f60f324bdb22108a7b36657d8473d913f139
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103815"
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