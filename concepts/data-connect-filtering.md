---
title: Microsoft Graph 数据连接中的用户选择和筛选功能
description: 介绍了如何使用 Microsoft Graph 数据连接来选择用户以提取其数据，以及筛选返回的数据。
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: cfe05545a6cfacc08f132be37c54c3a31ccdd62a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139182"
---
# <a name="user-selection-and-filtering-capabilities-in-microsoft-graph-data-connect"></a>Microsoft Graph 数据连接中的用户选择和筛选功能

你可以使用 Microsoft Graph 数据连接来选择要提取其数据的用户，并包含筛选器以限制返回的数据。 本文介绍数据连接提供的用户选择选项，以及它支持的筛选功能。

## <a name="user-selection"></a>用户选择

可以针对一组用户运行管道。 下面是适用于用户选择的选项：

- 组织内的所有用户
- 对组织内最多 10 个用户组运行
- 基于由 Azure Active Directory 用户属性组成的谓词的一组用户。

在 Azure 数据工厂复制活动的 SourceDataSet 中指定用户选择。 若要针对组列表运行，请在 **typeProperties** 下添加一个新字段 **allowedGroups**，并将此字段设置为最多 10 个组的列表，**对象 Id** 由逗号分隔。 如果默认情况下未指定组，则将为整个组织提取数据。

若要指定针对整个租户运行的谓词，请在 **typeProperties** 下添加一个新字段 **userScopeFilterUri**，并将此字段设置为该谓词。 谓词格式应与 Microsoft Graph API 的查询格式匹配。 例如，如果要仅选择在财务部门工作的用户，你可以使用 `https://graph.microsoft.com/v1.0/users?$filter=Department eq 'Finance'`。 如果要仅选择一个用户，可使用 `https://graph.microsoft.com/v1.0/users?$filter=mail eq 'contosouser1@contoso.com'`。

查询将仅返回你所查询的 Microsoft 365 组织内的用户。 将不会返回来宾用户和非用户邮箱。

## <a name="filtering"></a>筛选

可以使用日期时间属性来限制查询提取到的结果。 根据所请求数据的类型，可能需要日期时间筛选器。 日期时间筛选器使用的属性由 Azure 数据工厂复制活动的 SourceDataSet 提供。 若要指定日期时间筛选器，请在 **typeProperties** 下添加一个新字段 **dateFilterColumn**，并将此字段设置为下表中支持筛选的属性之一。 接着，添加表示日期时间值的 **startTime** 和 **endTime**，系统将依据这些值对属性进行筛选。

以下数据集需要针对相应的其中一个日期时间属性提供筛选器。

| 数据集名称                                               | 支持筛选的属性                                           |
| ---------------------------------------------------------- | --------------------------------------------------------------------------- |
| BasicDataSet_v0.Event_v0<br>BasicDataSet_v0.Event_v1       | CreatedDateTime<br>LastModifiedDateTime                                     |
| BasicDataSet_v0.Message_v0<br>BasicDataSet_v0.Message_v1   | CreatedDateTime<br>LastModifiedDateTime<br>ReceivedDateTime<br>SentDateTime |
| BasicDataSet_v0.SentItem_v0<br>BasicDataSet_v0.SentItem_v1 | CreatedDateTime<br>LastModifiedDateTime<br>ReceivedDateTime<br>SentDateTime |

> [!NOTE]
> 请求 BasicDataSet_v0.CalendarView_v0 的管道也需要日期时间筛选器，但 SourceDataSet 中未指定 **dateFilterColumn**。 但是，需要 **startTime** 和 **endTime**，且只提供了在 **startTime** 之后开始并在 **endTime** 之前完成的事件。

## <a name="see-also"></a>另请参阅

- [与 PAM 集成](data-connect-pam.md)
- [数据连接常见问题解答](data-connect-faq.md)
