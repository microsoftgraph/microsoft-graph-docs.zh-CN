---
title: 管理重点收件箱
description: '重点收件箱允许你查看"收件箱"选项卡中的重要邮件，以及选项卡中的其余 `Focused` "收件箱" `Other` 邮件。分类系统 '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 3f30bab46d1f51babc0064b22dfa8ce6975b0a2c7f86e53107ee77b59ae1a920
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141467"
---
# <a name="manage-focused-inbox"></a>管理重点收件箱

命名空间：microsoft.graph

通过重点收件箱，你可以查看收件箱的 `Focused` 选项卡中的重要邮件和 `Other` 选项卡中的其余收件箱邮件。分类系统最初按照默认方式组织收件箱邮件。可以随着时间推移通过用户界面或以编程方式对系统进行更正和培训。使用地越多，系统越能更好地推断哪些传入邮件是重要的。

在编程级别，重点收件箱 REST API 适用于指定用户的邮件，并支持每个邮件的 **inferenceClassification** 属性。可能的值为 `Focused` 和 `Other`，分别指示用户是否将邮件视为较重要和不太重要。若要更正系统对邮件进行分类的方式，请 [更新此邮件的 inferenceClassification 属性](../api/message-update.md)。随着时间的推移，这些更正也能对邮件分类系统进行培训。

重点收件箱 REST API 还使你能够创建替代。由 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 实例表示的每个替代，会指示分类系统始终以一致的方式指定来自特定发件人的邮件（即，始终作为“重点”或“其他”），而与任何以前的学习方法无关。可以 [创建](../api/inferenceclassification-post-overrides.md)、[列出](../api/inferenceclassification-list-overrides.md)、[更新](../api/inferenceclassificationoverride-update.md) 和 [删除](../api/inferenceclassificationoverride-delete.md) 指定用户的替代。可以在 **inferenceClassification** 导航属性中访问该用户的替代（如有），这些替代是 **inferenceClassificationOverride** 实例的集合。替代使用户能够更好地控制传入邮件的分类，并提高分类系统的可靠性。

注意，分类系统学习分类并仅对收件箱中的传入邮件应用分类。默认情况下，其他文件夹中的邮件为“重点”邮件。设置替代会影响以后到达收件箱的邮件；替代不会修改任意文件夹（包括收件箱）中现有邮件的 **inferenceClassification** 属性。

## <a name="focused-inbox-api"></a>重点收件箱 API

**对邮件分类系统进行培训**

[更新邮件的 inferenceClassification 属性](../api/message-update.md)


**使用替代对每个发件人一致分类**

[创建发件人替代](../api/inferenceclassification-post-overrides.md) | [列出所有用户替代](../api/inferenceclassification-list-overrides.md) |

[更新发件人替代](../api/inferenceclassificationoverride-update.md) | [删除发件人替代](../api/inferenceclassificationoverride-delete.md)

