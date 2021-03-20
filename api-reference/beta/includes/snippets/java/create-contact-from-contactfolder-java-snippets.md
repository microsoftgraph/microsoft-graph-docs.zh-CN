---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f73bde00d8d91dc5cd0d2244f793406752f086a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978933"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = new Contact();
contact.parentFolderId = "parentFolderId-value";
contact.birthday = OffsetDateTimeSerializer.deserialize("2016-10-19T10:37:00Z");
contact.fileAs = "fileAs-value";
contact.displayName = "displayName-value";
contact.givenName = "givenName-value";
contact.initials = "initials-value";

graphClient.me().contactFolders("{id}").contacts()
    .buildRequest()
    .post(contact);

```