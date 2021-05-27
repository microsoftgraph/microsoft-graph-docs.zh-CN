---
title: 使用连接器 API
description: Microsoft Graph 连接器 API 概述
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 63e11b086592a46a4e519a2ab7c79c20d049213a
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645902"
---
# <a name="working-with-the-connectors-api"></a>使用连接器 API

Microsoft Graph 连接器平台提供了一种简单的方法，可将外部数据添加到 Microsoft Graph 中并提升 Microsoft 365 智能体验。 你可能希望构建自定义连接器，以与未作为 Microsoft 构建的连接器的服务集成。 若要构建自定义连接器，请使用 Microsoft Graph 连接器 REST API。

![图像显示外部数据即将通过不同类型的连接线连接到 Microsoft Graph](./images/connectors-images/api-overview.png)

可以使用 Microsoft Graph 连接器 API 来：

1. 创建和管理外部数据连接。
2. 定义和注册外部数据类型的架构。
3. 将外部数据项提取到 Microsoft Graph 中。
4. 同步外部组。

如果要了解有关这些 API 的更多详细信息，可以访问下面建议的文档。

## <a name="connections-api"></a>连接 API

连接是外部数据的逻辑容器，您可以作为一个单元进行管理。
如果要了解有关如何在 Microsoft Graph 中创建、更新和删除连接的更多信息，请访问[管理连接](connecting-external-content-manage-connections.md)部分。

## <a name="schema-api"></a>架构 API

连接[架构](/graph/api/resources/schema?view=graph-rest-beta&amp;preserve-view=true)确定各种 Microsoft 365 体验中如何使用你的内容。 架构是计划添加到连接中的所有属性的简单列表及其属性、标签和别名。 必须先注册架构，然后才能将项目提取到 Microsoft Graph 中。

如果要了解有关如何为 Microsoft Graph 连接注册架构及其属性的更多信息，请访问[管理架构](connecting-external-content-manage-schema.md)部分。

## <a name="ingest-external-data-items"></a>提取外部数据项

Microsoft Graph 连接器平台提供了一种简单的方法，可将外部数据添加到 Microsoft Graph 中。 应用程序添加到 Microsoft 搜索服务的项用 Microsoft Graph 中的 [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) 资源表示。

如果要了解有关如何创建、更新和删除应用程序通过 Microsoft Graph 连接器添加的项目的更多信息，请访问[管理项目](connecting-external-content-manage-items.md)部分。

## <a name="external-groups-api"></a>外部组 API

可通过 ACL 对不同类型的非 Azure Active Directory 组授予或拒绝对外部服务中的项目的访问。 例如，Salesforce 项可能拥有权限集和配置文件。 ServiceNow 项目可能有本地组。 将这些项目提取到 Microsoft Graph 中时，需要遵守这些 ACL。

可以使用外部组 API 来设置对提取到 Microsoft Graph 中的外部项目权限。 [externalGroup](/graph/api/externalgroup-post-members?view=graph-rest-beta&amp;preserve-view=true) 表示非 Azure Active Directory 组或类似组的构造（例如业务部门、团队等），并确定对外部数据源中内容的权限。