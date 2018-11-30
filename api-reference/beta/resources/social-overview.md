---
title: 使用 Microsoft Graph API 将应用程序中的社交智能集成
description: Microsoft Graph 社交手势支持在用户的社交上下文中，并提供对有用的个人和社会数据访问。
ms.openlocfilehash: b83c5ea08c6d66dc800f736717f50324f0e2b4b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047300"
---
# <a name="use-the-microsoft-graph-api-to-integrate-social-intelligence-in-an-app"></a>使用 Microsoft Graph API 将应用程序中的社交智能集成

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

Microsoft Graph 社交手势支持在用户的社交上下文中，并提供对有用的个人和社会数据访问。

## <a name="aggregate-and-extract-specific-information-about-people"></a>聚合和提取人员相关的特定信息

使用邮件、 联系人和社交网络之间的[人员](../resources/person.md)资源和此人的聚合信息的人员 API。 按其相关性基于多个通信、 协作和业务关系，对结果进行排序。 API 可以浏览、 排序、 选择、 筛选器或按条件的人员搜索。

- [List people](../api/user-list-people.md)

## <a name="manage--mentions"></a>管理 @ 提及

调用出收件人通知和消息中获取收件人的注意是常见的社交笔势。
[提及](../resources/mention.md)资源和提到 API 提供细线的机制来呼叫出中[邮件](../resources/message.md)的收件人，获取在其中使用 @-提及，通知用户的所有邮件，或都获取一条消息中的每个提及。

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- 创建新邮件中提及

  - [创建和发送提及作为新邮件的一部分](../api/user-sendmail.md#request-2)
  - [创建提及的邮件草稿一部分](../api/user-post-messages.md#request-2)

- 在邮件中获取提及相关信息

  - [获取提及用户的登录用户邮箱中的所有邮件](../api/user-list-messages.md#request-2)
  - [获取一条消息中的每个提及的详细信息](../api/message-get.md#request-2)

- 在邮件中[删除某个提及](../api/message-delete.md#request-2)

## <a name="access-social-data-around-and-about-a-user"></a>围绕用户以及访问社交数据

Office 图形封装在 Office 365 中的不同实体之间的关系。 使用 Office 图形跨 Office 365 中获取单个用户的社交见解。

- 列表项[趋势围绕](../api/insights-list-trending.md)用户
- 列出用户的已[处理](../api/user-list-people.md)的用户
