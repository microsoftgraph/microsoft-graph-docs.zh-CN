---
title: 使用 Microsoft Graph 连接器 API
description: 使用 Microsoft Graph 连接器 API 构建自定义连接器，将外部数据引入到 Microsoft Graph 中以增强 Microsoft 365 智能体验。
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 4c2359f7e565b9d1ff00e623649e833363fc6231
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094415"
---
# <a name="work-with-the-microsoft-graph-connectors-api"></a>使用 Microsoft Graph 连接器 API

Microsoft Graph 连接器将外部数据引入到 Microsoft Graph 中并增强 Microsoft 365 智能体验。 你可能希望构建自定义连接器，以与未作为 Microsoft 构建的连接器的服务集成。 若要构建自定义连接器，请使用 Microsoft Graph 连接器 REST API。

![图像显示外部数据即将通过不同类型的连接线连接到 Microsoft Graph](./images/connectors-images/api-overview.png)

可以使用 Microsoft Graph 连接器 API 来：

1. 创建和管理外部数据连接。
2. 定义和注册外部数据类型的架构。
3. 将外部数据项提取到 Microsoft Graph 中。
4. 同步外部组。

## <a name="create-and-manage-external-data-connections"></a>创建和管理外部数据连接

[externalConnection](/graph/api/resources/externalconnectors-externalconnection) 资源（外部连接 API）是外部数据的逻辑容器，可将其作为单一单元进行管理。

要了解详细信息，请参阅 [创建、更新和删除 Microsoft Graph 中的连接](connecting-external-content-manage-connections.md)。

## <a name="define-and-register-the-schema-of-the-external-data-types"></a>定义和注册外部数据类型的架构

连接[架构](/graph/api/resources/externalconnectors-schema) (架构 API) 确定如何在各种 Microsoft 365 体验中使用内容。 架构是计划与其特性、标签和别名一起添加到连接中的所有属性的简单列表。 必须先注册架构，然后才能将项目提取到 Microsoft Graph 中。

要了解详细信息，请参阅 [注册并更新 Microsoft Graph 连接的架构](connecting-external-content-manage-schema.md)。

## <a name="ingest-external-data-items-into-microsoft-graph"></a>将外部数据项提取到 Microsoft Graph 中

应用程序添加到 Microsoft 搜索服务的项目由 Microsoft Graph 中的 [externalItem](/graph/api/resources/externalconnectors-externalitem) 资源（外部项目 API）表示。

要了解详细信息，请参阅 [通过 Microsoft Graph 连接器创建、更新和删除应用程序添加的项目](connecting-external-content-manage-items.md)。

## <a name="sync-external-groups"></a>同步外部组

可通过 ACL 对不同类型的非 Azure Active Directory 组授予或拒绝对外部服务中的项目的访问。 例如，Salesforce 项可能具有权限集和配置文件，而 ServiceNow 项可能具有本地组。 将这些项目提取到 Microsoft Graph 中时，需要遵守这些 ACL。

可以使用外部组 API 来设置对提取到 Microsoft Graph 中的外部项的权限。 [externalGroup](/graph/api/resources/externalconnectors-externalgroup) 表示非 Azure Active Directory 组或类似组的构造（例如业务部门、团队等），并确定对外部数据源中内容的权限。

要了解详细信息，请参阅 [使用外部组管理对 Microsoft Graph 连接器数据源的权限](connecting-external-content-external-groups.md)。

## <a name="next-steps"></a>后续步骤

- [生成自定义连接器](/graph/connecting-external-content-build-quickstart)