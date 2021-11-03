---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b36641806a8f48043d3802c62575a806c4f30aa5c2b692c08fdecd073a7b466
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278496"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemReference sourceFile = new ItemReference();
SharepointIds sharepointIds = new SharepointIds();
sharepointIds.listId = "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0";
sharepointIds.listItemId = "2";
sourceFile.sharepointIds = sharepointIds;

String destinationFileName = "newname.txt";

graphClient.sites("{id}").contentTypes("{contentTypeId}")
    .copyToDefaultContentLocation(ContentTypeCopyToDefaultContentLocationParameterSet
        .newBuilder()
        .withSourceFile(sourceFile)
        .withDestinationFileName(destinationFileName)
        .build())
    .buildRequest()
    .post();

```