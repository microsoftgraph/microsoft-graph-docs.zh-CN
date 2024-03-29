---
title: 使用 Outlook 邮件 API 组织 Outlook 邮件
description: 按照你喜欢的方式组织 Outlook 邮件。 方便地对整个邮箱或特定文件夹中的邮件进行筛选、搜索或排序。
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: e2c098234e1ea37e98e22153e56b6d88783e9f0c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444318"
---
# <a name="organize-outlook-messages"></a>整理 Outlook 邮件

Outlook 允许客户按照自己喜欢的方式整理邮件，可以将所有邮件都留在同一“收件箱”文件夹中，或者在“收件箱”下的树文件夹结构中整理邮件，以满足自己的特定需要。 可以方便地对用户整个邮箱或特定文件夹中的邮件进行[筛选、搜索或排序](query-parameters.md)。

## <a name="access-mail-folders"></a>访问邮件文件夹

以编程方式，邮件文件夹由 [mailFolder](/graph/api/resources/mailfolder) 资源表示，“收件箱”是文件夹结构根目录中的一个文件夹。

每个 **mailFolder** 都由其文件夹 ID 标识，并具有可写的 **displayName** 属性。 Outlook 默认情况下会为客户创建其他几个文件夹。 可以按文件夹 ID 或其已知的名称引用这些默认文件夹。 有关可用的已知文件夹名称的列表，请参阅 [mailFolder 资源类型](/graph/api/resources/mailfolder)。

对于自定义的非默认文件夹，如果知道其文件夹路径，则可先使用 `/users/{id}/mailfolders` 快捷方式进入根级别并获取所有顶级文件夹，以访问该文件夹：

```http
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders
```

然后，在浏览文件夹树的每个级别时指定相应的文件夹 ID (`{folder_id}`)：

```http
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders/{folder_id}/childfolders
```

重复此操作，直到最终到达树中的自定义文件夹。

## <a name="create-and-organize-the-folder-tree"></a>创建和组织文件夹树

可以 [在“收件箱”下创建邮件文件夹](/graph/api/user-post-mailfolders)，或者作为 [其他文件夹的子文件夹](/graph/api/mailfolder-post-childfolders)。 创建、[复制](/graph/api/mailfolder-copy)或 [移动](/graph/api/mailfolder-move)文件夹及其内容时，Outlook 会更新所涉及文件夹的只读 **parentFolderId** 和 **childFolderCount** 属性。 当文件夹的内容复制或移动到另一个文件夹时，默认情况下，内容的各个条目 ID 也会更改。

在内容级别，**totalItemCount** 和 **unreadItemCount** 分别告诉你邮件文件夹中的项目数和未读项目数。
在子文件夹级别，可以[列出“收件箱”或任何其他文件夹下的子文件夹](/graph/api/user-list-mailfolders)。
**childFolderCount** 属性表示直接子文件夹的数量。

请注意，Outlook 邮件文件夹可以包含邮件和非邮件项目，例如事件和联系人。 通常，Outlook 文件夹可以包含异类项目。

## <a name="use-rules-to-automate-copying-or-moving-messages"></a>使用规则自动复制或移动邮件

Outlook 允许客户设置规则，以在满足某些预确定的条件时自动对传入邮件执行特定操作。 可以为“收件箱”[创建一个规则](/graph/api/mailfolder-post-messagerules)作为 [messageRule](/graph/api/resources/messagerule)，以在特定条件下将邮件复制或移动到特定文件夹。
条件是 [messageRulePredicates](/graph/api/resources/messagerulepredicates)。 它们可以包括包含特定文本的邮件主题或正文、从某些电子邮件地址发送的邮件或标记为重要的邮件等等。

## <a name="direct-only-the-messages-you-care-about-to-the-focused-inbox"></a>仅将你关注的邮件定向到重点收件箱

“重点收件箱”可让客户训练 Outlook 在“**重点**”选项卡中仅显示来自关注发件人传入的邮件，其余邮件则在“**其他**”选项卡上。最初，Outlook 的分类系统以默认方式整理“收件箱”邮件。 随着时间的推移，可以通过用户界面或以编程方式对系统进行更正和训练。 使用“重点收件箱”越多，分类系统就能越好推断出要在“**重点**”选项卡上查看的传入邮件。

通过编程方式，可以更新 [邮件](/graph/api/resources/message)的 **inferenceClassification** 属性，以指示要在“重点”还是“其他”选项卡中查看邮件。这是特定邮件的一次性指定。 另一方面，如果希望始终在“重点”选项卡或“其他”选项卡中查看来自特定发件人的邮件，则可以为 Outlook [设置指令](/graph/api/inferenceclassification-post-overrides)。 每条指令都是一个 [inferenceClassificationOverride](/graph/api/resources/inferenceclassificationoverride) 实例，指定发件人的姓名，并指定来自该发件人的邮件始终为 `focused` 或 `other`。 对用户“重点收件箱”的每条用户指令都存储为 [user](/graph/api/resources/user) 对象的一个 [inferenceClassificationOverride](/graph/api/resources/inferenceclassificationoverride) 实例集合。

## <a name="keep-messages-and-mail-folders-up-to-date-in-apps"></a>在应用中使邮件和邮件文件夹保持最新

应用通常必须同步并在应用本地存储中使用户的邮件数据保持最新。 Microsoft Graph 允许订阅更改通知，以在数据更改时得到通知，并在发生更改时立即查询实际更改。

在发生更改时，通知将通过 [webhooks](/graph/api/resources/webhooks) 异步传递，从而节省应用频繁进行轮询的开销。 可以[订阅有关添加、更新或删除用户邮件数据的更改通知](/graph/api/subscription-post-subscriptions)。 例如，可以创建对特定文件夹（即 `/me/mailFolders('{folderId'}')`）或根级别（即 `/me/messages`）中邮件的订阅。 订阅会指定一个 **notificationUrl**，Microsoft Graph 将在发生所请求类型的更改时在其中通知应用。

若要初始同步用户的邮箱，首先，请[对从根级别开始的邮件文件夹执行增量查询](/graph/api/mailfolder-delta)，以同步所有邮件文件夹，然后[对每个文件夹中的邮件执行增量查询](/graph/api/message-delta)，以同步各个邮件。

若要查找在未通过任何通知读取整个资源的情况下更改的确切实体，可以使用[增量查询](delta-query-overview.md)跟踪重要更改，并将本地存储与这些更改同步。 可以[跟踪特定文件夹中的邮件更改](delta-query-messages.md)。 还可以跟踪根级别（即 `/me/mailfolders`）的邮件文件夹更改。

## <a name="next-steps"></a>后续步骤

- [为什么与 Outlook 邮件集成](outlook-mail-concept-overview.md)
- 在 Microsoft Graph v1.0 中 [使用邮件 API](/graph/api/resources/mail-api-overview) 及其 [用例](/graph/api/resources/mail-api-overview#common-use-cases)
