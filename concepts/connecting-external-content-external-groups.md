---
title: 使用外部组管理对 Microsoft Graph连接器数据源的权限
description: 了解用于管理外部项权限的外部组。
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 8a0ae00e7fc4d1509c29bfb204aae0ab3166970e
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781185"
---
# <a name="use-external-groups-to-manage-permissions-to-microsoft-graph-connector-data-sources"></a><span data-ttu-id="534e4-103">使用外部组管理对 Microsoft Graph连接器数据源的权限</span><span class="sxs-lookup"><span data-stu-id="534e4-103">Use external groups to manage permissions to Microsoft Graph connector data sources</span></span>

<span data-ttu-id="534e4-104">[外部组](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true)允许你管理查看 Microsoft Graph[](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)连接中的外部项以及连接到 Azure AD) 组外部Azure Active Directory (的权限。</span><span class="sxs-lookup"><span data-stu-id="534e4-104">[External groups](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) allow you to manage permissions to view [external items](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) in a Microsoft Graph connection, and connect to data sources outside Azure Active Directory (Azure AD) groups.</span></span>

<span data-ttu-id="534e4-105">对于依赖 Azure AD 用户和组的数据源，在创建或更新外部项时，通过将访问控制列表 (ACL) 与 Azure AD 用户和组 ID 关联来设置外部[](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true)项的权限。</span><span class="sxs-lookup"><span data-stu-id="534e4-105">For data sources that rely on Azure AD users and groups, you set permissions on external items by associating an access control list (ACL) with an Azure AD user and group ID, when [creating](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true) or updating the external items.</span></span>

<span data-ttu-id="534e4-106">但是，对于使用非 Azure AD 组或类似组构造的数据源（如 Salesforce 配置文件、Dynamics 业务部门、SharePoint 组、ServiceNow 本地组或 Confluence 本地组）我们建议使用外部 *组*。</span><span class="sxs-lookup"><span data-stu-id="534e4-106">However, for data sources that use non-Azure AD groups, or group-like constructs, like Salesforce Profiles, Dynamics Business Units, SharePoint groups, ServiceNow local groups, or Confluence local groups, we recommend that you use *external groups*.</span></span>

## <a name="common-external-group-scenarios"></a><span data-ttu-id="534e4-107">常见的外部组方案</span><span class="sxs-lookup"><span data-stu-id="534e4-107">Common external group scenarios</span></span>

<span data-ttu-id="534e4-108">以下是常见的非 Azure AD 应用程序特定的组示例。</span><span class="sxs-lookup"><span data-stu-id="534e4-108">The following are common non-Azure AD application-specific group examples.</span></span>

<span data-ttu-id="534e4-109">Microsoft Dynamics 365 允许客户使用业务部门和团队构建其 CDM。</span><span class="sxs-lookup"><span data-stu-id="534e4-109">Microsoft Dynamics 365 allows customers to structure their CRMs with business units and teams.</span></span><span data-ttu-id="534e4-110">这些业务部门和团队的成员身份信息未存储在 Azure AD 中。</span><span class="sxs-lookup"><span data-stu-id="534e4-110"> The membership information for these business units and teams is not stored in Azure AD.</span></span>

<span data-ttu-id="534e4-111">下图显示了业务部门和团队的结构。</span><span class="sxs-lookup"><span data-stu-id="534e4-111">The following image shows the structure of the business units and teams.</span></span>

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/bu-teams-D365.png" alt="Diagram of an structure in Dynamics 365. A business unit has a team and a manager under it. This manager has other users." style="width:400px;"/></p>

<span data-ttu-id="534e4-112">Salesforce 使用配置文件、角色和权限集进行授权。</span><span class="sxs-lookup"><span data-stu-id="534e4-112">Salesforce uses profiles, roles, and permission sets for authorization.</span></span> <span data-ttu-id="534e4-113">这些信息特定于 Salesforce，并且成员身份信息在 Azure AD 中不可用。</span><span class="sxs-lookup"><span data-stu-id="534e4-113">These are specific to Salesforce, and the membership information is not available in Azure AD.</span></span>

<span data-ttu-id="534e4-114">下图显示了 Salesforce 中成员身份信息的结构。</span><span class="sxs-lookup"><span data-stu-id="534e4-114">The following image shows the structure of the membership information in Salesforce.</span></span>

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/roles-salesforce.png" alt="Diagram of an structure of roles in Salesforce. The role of vicepresident of sales is at the top level of the hierarchy, it has three subordinates, namely, the head of sales operations, the head of sales, and the head of account managament. The head of sales at the same time has a sales operations manager as subordinate. And the head of sales has a sales development manager as subordinate." style="width:400px;"/></p>

## <a name="using-external-groups-in-your-connection"></a><span data-ttu-id="534e4-115">在连接内使用外部组</span><span class="sxs-lookup"><span data-stu-id="534e4-115">Using external groups in your connection</span></span>

<span data-ttu-id="534e4-116">若要在连接内使用外部组：：</span><span class="sxs-lookup"><span data-stu-id="534e4-116">To use external groups in your connections:</span></span>

1. <span data-ttu-id="534e4-117">对于每个非 Azure AD 组，使用组 API 在 Microsoft Graph创建[外部组](/en-us/graph/api/resources/group?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="534e4-117">For each non-Azure AD group, create an external group in Microsoft Graph using the [groups API](/en-us/graph/api/resources/group?view=graph-rest-beta&preserve-view=true).</span></span>
2. <span data-ttu-id="534e4-118">必要时，在定义外部项的 ACL 时，请使用外部组。</span><span class="sxs-lookup"><span data-stu-id="534e4-118">Use the external group when defining the ACL for your external items as necessary.</span></span>  
3. <span data-ttu-id="534e4-119">使外部组的成员身份保持最新并同步。</span><span class="sxs-lookup"><span data-stu-id="534e4-119">Keep the membership of the external groups up to date and in sync.</span></span>

### <a name="create-external-groups"></a><span data-ttu-id="534e4-120">创建外部组</span><span class="sxs-lookup"><span data-stu-id="534e4-120">Create external groups</span></span>

<span data-ttu-id="534e4-121">外部组属于连接。</span><span class="sxs-lookup"><span data-stu-id="534e4-121">External groups belong to a connection.</span></span> <span data-ttu-id="534e4-122">若要在连接内创建外部组，请：</span><span class="sxs-lookup"><span data-stu-id="534e4-122">To create external groups in your connections:</span></span>
* <span data-ttu-id="534e4-123">使用 Microsoft Graph中的组 API，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="534e4-123">Use the groups API in Microsoft Graph, as shown in the following example.</span></span>

    > [!NOTE]
    > <span data-ttu-id="534e4-124">[displayName 和](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) **description** 是可选的字段。</span><span class="sxs-lookup"><span data-stu-id="534e4-124">The [displayName](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) and **description** are optional fields.</span></span>

    ```http
    POST /connections/{connectionId}/groups 

    {  
      "id": "contosoEscalations",  
      "displayName": "Contoso Escalations",  
      "description": "Tier-1 escalations within Contoso"
    }  
    ```

* <span data-ttu-id="534e4-125">在 ID 字段中提供 [标识符或名称](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) 。</span><span class="sxs-lookup"><span data-stu-id="534e4-125">Provide either an identifier or a name in the [ID](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) field.</span></span> <span data-ttu-id="534e4-126">使用此值在后续请求中调用外部组。</span><span class="sxs-lookup"><span data-stu-id="534e4-126">Use this value to call the external group in subsequent requests.</span></span>

    > [!NOTE]
    > <span data-ttu-id="534e4-127">ID 字段允许您使用 URL 和 filename-safe Base64 字符集，其限制为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="534e4-127">The ID field allows you to use URL and filename-safe Base64 character sets, and it has a limit of 128 characters.</span></span>

<span data-ttu-id="534e4-128">外部组可以包含以下一个或多个：</span><span class="sxs-lookup"><span data-stu-id="534e4-128">An external group can contain one or more of the following:</span></span>
* <span data-ttu-id="534e4-129">Azure AD 用户。</span><span class="sxs-lookup"><span data-stu-id="534e4-129">An Azure AD user.</span></span>
* <span data-ttu-id="534e4-130">Azure AD 组。</span><span class="sxs-lookup"><span data-stu-id="534e4-130">An Azure AD group.</span></span>
* <span data-ttu-id="534e4-131">另一个外部组，包括嵌套外部组。</span><span class="sxs-lookup"><span data-stu-id="534e4-131">Another external group, including nested external groups.</span></span>

<span data-ttu-id="534e4-132">创建组后，可以将成员添加到组，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="534e4-132">After you create the group, you can add members to the group, as shown in the following examples.</span></span>

```http
POST https://graph.microsoft.com/beta/connections/{connectionId}/groups/{groupId}/members

{ 
  "id": "contosoSupport", 
  "type": "group", 
  "identitySource": "external" 
}
```
```http
POST https://graph.microsoft.com/beta/connections/{connectionId}/groups/{groupId}/members 

{ 
  "id": "25f143de-be82-4afb-8a57-e032b9315752", 
  "type": "user", 
  "identitySource": "azureActiveDirectory" 
}
```
```http
POST https://graph.microsoft.com/beta/connections/{connectionId}/groups/{groupId}/members 

{ 
  "id": "99a3b3d6-71ee-4d21-b08b-4b6f22e3ae4b", 
  "type": "group", 
  "identitySource": "azureActiveDirectory" 
}
```

### <a name="use-external-groups-in-acl"></a><span data-ttu-id="534e4-133">在 ACL 中使用外部组</span><span class="sxs-lookup"><span data-stu-id="534e4-133">Use external groups in ACL</span></span>

<span data-ttu-id="534e4-134">定义外部项的 [ACL](connecting-external-content-manage-items.md#access-control-list) 时，可以使用外部组，如以下示例所示。</span><span class="sxs-lookup"><span data-stu-id="534e4-134">You can use external groups when defining [ACLs](connecting-external-content-manage-items.md#access-control-list) for external items, as shown in the following example.</span></span> <span data-ttu-id="534e4-135">除了 Azure AD 用户和组外，外部项的访问控制条目中还可以包含外部组。</span><span class="sxs-lookup"><span data-stu-id="534e4-135">In addition to Azure AD users and groups, an external item can have external groups in its access control entries.</span></span>

```http
PUT https://graph.microsoft.com/beta/external/connections/{id}/items/{id}  

Content-type: application/json  
{  
  "@odata.type": "microsoft.graph.externalItem",  
  "acl": [  
    {  
      "type": "group",  
      "value": "contosEscalations",  
      "accessType": "grant",  
      "identitySource": "External"  
    },  
    {  
      "type": "user",  
      "value": "87e9089a-08d5-4d9e-9524-b7bd6be580d5",  
      "accessType": "grant",  
      "identitySource": "azureActiveDirectory"  
    },  
    {  
      "type": "group",  
      "value": "96fbeb4f-f71c-4405-9f0b-1d6988eda2d2",  
      "accessType": "deny",  
      "identitySource": "azureActiveDirectory"  
    }  
  ],  
  "properties": {  
    "title": "Error in the payment gateway",  
    "priority": 1,  
    "assignee": "john@contoso.com"  
  },  
  "content": {  
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>",  
    "type": "html"  
  }  
}  
```

> [!NOTE]
> <span data-ttu-id="534e4-136">即使在创建外部组之前，您也可在 ACL 中使用这些外部组。</span><span class="sxs-lookup"><span data-stu-id="534e4-136">You can use external groups in ACLs even before the groups are created.</span></span>

### <a name="keep-external-group-memberships-in-sync"></a><span data-ttu-id="534e4-137">保持外部组成员身份同步</span><span class="sxs-lookup"><span data-stu-id="534e4-137">Keep external group memberships in sync</span></span>

<span data-ttu-id="534e4-138">在 Microsoft Graph 中保持外部组的成员身份Graph。</span><span class="sxs-lookup"><span data-stu-id="534e4-138">Keep the membership of your external group up to date in Microsoft Graph.</span></span> <span data-ttu-id="534e4-139">当自定义组的成员身份更改时，请确保更改在满足你需求的一个时间反映在外部组中。</span><span class="sxs-lookup"><span data-stu-id="534e4-139">When memberships change in your custom group, make sure that the change is reflected in the external group at a time that works for your needs.</span></span>

### <a name="manage-external-groups-and-membership"></a><span data-ttu-id="534e4-140">管理外部组和成员身份</span><span class="sxs-lookup"><span data-stu-id="534e4-140">Manage external groups and membership</span></span>

<span data-ttu-id="534e4-141">可以使用组 API 管理外部组和组成员身份。</span><span class="sxs-lookup"><span data-stu-id="534e4-141">You can use the groups API to manage your external groups and group membership.</span></span> <span data-ttu-id="534e4-142">有关详细信息，请参阅 [externalGroup](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) 和 [externalGroupMember](/graph/api/resources/externalgroupmember?view=graph-rest-beta&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="534e4-142">For details, see [externalGroup](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) and [externalGroupMember](/graph/api/resources/externalgroupmember?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="see-also"></a><span data-ttu-id="534e4-143">另请参阅</span><span class="sxs-lookup"><span data-stu-id="534e4-143">See also</span></span>
<span data-ttu-id="534e4-144">若要了解有关 Microsoft Graph 连接器 API 的更多信息，请参阅[使用连接器 API。](connecting-external-content-connectors-api-overview.md)</span><span class="sxs-lookup"><span data-stu-id="534e4-144">To learn more about the Microsoft Graph connectors API, see [Working with the connectors API](connecting-external-content-connectors-api-overview.md).</span></span>
