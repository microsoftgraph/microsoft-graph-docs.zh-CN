---
title: 用户选择和筛选 Microsoft Graph 数据连接支持
description: 介绍如何使用 Microsoft Graph 数据连接来选择用户以提取其数据，以及筛选返回的数据。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 1d558c441a626a312d0097d143d194255aaed769
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629836"
---
# <a name="user-selection-and-filtering-microsoft-graph-data-connect-supports"></a>用户选择和筛选 Microsoft Graph 数据连接支持

你可以使用 Microsoft Graph 数据连接来选择要提取其数据的用户，并包括筛选器以限制返回的数据。 本文介绍数据连接提供的用户选择选项，以及它支持的筛选。 

## <a name="user-selection"></a>用户选择 

可以针对一组用户运行管道。 下面是适用于用户选择的选项：
- 组织内的所有用户
- 组织内要针对其运行的最多 10 个用户组 
- 基于由 Azure Active Directory 用户属性组成的谓词的一组用户。

在 Azure 数据工厂复制活动的 SourceDataSet 中指定用户选择。 若要针对组列表运行，请在 **typeProperties** 下添加一个新字段 **allowedGroups**，并将此字段设置为最多 10 个组的**对象 Id** 组成的列表，由逗号分隔。 如果默认情况下未指定组，则将为整个组织提取数据。 

若要指定针对整个租户运行的谓词，请在 **typeProperties** 下添加一个新字段 **userScopeFilterUri**，并将此字段设置为该谓词。 谓词格式应与 Microsoft Graph API 的查询格式匹配。 例如，如果要仅选择在财务部门工作的用户，你可以使用 `https://graph.microsoft.com/v1.0/users?$filter=Department eq 'Finance'`。

查询将仅返回你所查询的 Office 365 组织内的用户。 将不会返回来宾用户和非用户邮箱。

## <a name="filtering"></a>筛选 

可以使用日期时间属性来限制为查询提取的结果。 根据所请求数据的类型，可能需要日期时间筛选器。 日期时间筛选器是使用 Azure 数据工厂复制活动的 SourceDataSet 中的属性提供的。 若要指定日期时间筛选器，请在 **typeProperties** 下添加一个新字段 **dateFilterColumn**，并将此字段设置为下表中支持筛选的属性之一。 接着，添加表示日期时间值的 **startTime** 和 **endTime**，系统将依据这些值对属性进行筛选。 

以下数据集需要在相应的日期时间属性之一上提供筛选器。

| 数据集名称                                                   | 支持筛选的属性                                           | 
|----------------------------------------------------------------|-----------------------------------------------------------------------------| 
| BasicDataSet_v0.Event_v0<br>BasicDataSet_v0.Event_v1           | CreatedDateTime<br>LastModifiedDateTime                                     | 
| BasicDataSet_v0.Message_v0<br>BasicDataSet_v0.Message_v1       | CreatedDateTime<br>LastModifiedDateTime<br>ReceivedDateTime<br>SentDateTime | 
| BasicDataSet_v0.SentItem_v0<br>BasicDataSet_v0.SentItem_v1     | CreatedDateTime<br>LastModifiedDateTime<br>ReceivedDateTime<br>SentDateTime |

>**注意：** 请求 BasicDataSet_v0.CalendarView_v0 的管道也需要日期时间筛选器，但 SourceDataSet 中未指定 **dateFilterColumn**。 但是，**startTime** 和 **endTime** 为必需，而只提供了在 **startTime** 之后开始并在 **endTime** 之前完成的事件。

## <a name="next-steps"></a>后续步骤 

有关如何修改为提取选择的用户以及在数据连接管道中进行筛选的详细信息，请参阅 [Azure 数据工厂 Office 365 连接器文档](https://docs.microsoft.com/zh-CN/azure/data-factory/connector-office-365)。  

  
