---
author: carolinetempleton
ms.topic: include
ms.localizationpriority: medium
ms.openlocfilehash: c17741c368295201dd626df91de161cf318efc1b
ms.sourcegitcommit: 0249c86925c9b4797908394c952073b5d9137911
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2022
ms.locfileid: "64477851"
---
<!-- markdownlint-disable MD041-->

### <a name="migrate-to-the-azure-resource-manager-arm-pim-api-for-azure-resource-roles"></a>迁移到 Azure 资源角色的 Azure 资源管理器 (ARM) PIM API

用于管理 Azure 资源的 PIM v3 API 现已通过 Azure 资源管理器 (ARM) REST API 提供。 使用本指南将现有 API 迁移到新的 [Azure 资源管理器 (ARM) API](/rest/api/authorization/privileged-role-eligibility-rest-sample)。

下表介绍了新 ARM API 如何映射到现有 API。

| Operation | Microsoft Graph API (PIM v2) | ARM API (PIM v3) |
| --------- | ------------ | -------------- |
| 注册资源 | [注册](/graph/api/governanceresource-register) | ARM 不需要显式注册或载入资源即可进行管理。 可以通过直接使用资源范围执行操作。 |
| 列出角色定义 | [列出角色定义](/graph/api/governanceroledefinition-list) | [角色定义 - 列表](/rest/api/authorization/role-definitions/list) |
| 创建角色分配请求 | [创建 governanceRoleAssignmentRequest](/graph/api/governanceroleassignmentrequest-post) | 使用 [角色资格计划请求 - 创建](/rest/api/authorization/role-eligibility-schedule-requests/create) 来创建符合条件的角色分配<br/><br/>使用 [角色分配计划请求 - 创建](/rest/api/authorization/role-assignment-schedule-requests/create) 来创建活动角色分配 |
| 列出角色分配 | [列出 governanceRoleAssignments](/graph/api/governanceroleassignment-list) | 使用 [角色资格计划实例 - 列表](/rest/api/authorization/role-eligibility-schedule-instances/list-for-scope) 获取符合条件的角色分配<br/><br/>使用 [角色分配计划实例 - 列表](/rest/api/authorization/role-assignment-schedule-instances/list-for-scope) 获取活动角色分配 |
| 管理角色设置 | [列出 governanceRoleSettings](/graph/api/governancerolesetting-list)<br/>[更新 governanceRoleSetting](/graph/api/governancerolesetting-update) | [通过 ARM 管理策略](/rest/api/authorization/privileged-role-policy-rest-sample)