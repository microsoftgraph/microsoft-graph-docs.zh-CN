---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 765d77839d39d054e72dfc5da128c7c4870cbd7a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094567"
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

graphClient.sites("microsoft.sharepoint.com,b9b0bc03-cbc4-40d2-aba9-2c9dd9821ddf,6a742cee-9216-4db5-8046-13a595684e74").termStore().sets("462bd0ae-30bb-4c58-845c-761ff6481ac1").terms()
    .buildRequest()
    .post(term);

```