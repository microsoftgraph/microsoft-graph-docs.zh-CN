---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3261bc7314cd46cf4353b14b5c9b2a10269e793
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973931"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Term term = new Term();
LinkedList<LocalizedLabel> labelsList = new LinkedList<LocalizedLabel>();
LocalizedLabel labels = new LocalizedLabel();
labels.languageTag = "en-US";
labels.name = "Car";
labels.isDefault = true;
labelsList.add(labels);
term.labels = labelsList;

graphClient.termStore().sets("{setId}").terms()
    .buildRequest()
    .post(term);

```