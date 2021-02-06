---
title: defaultUserRolePermissions 资源类型
description: 包含默认用户角色的某些可自定义权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b6ee2e8deccf73929b68079379efb0f6d93a3369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135672"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="ed260-103">defaultUserRolePermissions 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed260-103">defaultUserRolePermissions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed260-104">包含 Azure AD 中默认用户角色的某些可自定义权限。</span><span class="sxs-lookup"><span data-stu-id="ed260-104">Contains certains customizable permissions of default user role in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="ed260-105">属性</span><span class="sxs-lookup"><span data-stu-id="ed260-105">Properties</span></span>

| <span data-ttu-id="ed260-106">属性</span><span class="sxs-lookup"><span data-stu-id="ed260-106">Property</span></span> | <span data-ttu-id="ed260-107">类型</span><span class="sxs-lookup"><span data-stu-id="ed260-107">Type</span></span> | <span data-ttu-id="ed260-108">说明</span><span class="sxs-lookup"><span data-stu-id="ed260-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="ed260-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="ed260-109">allowedToCreateApps</span></span> | <span data-ttu-id="ed260-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed260-110">Boolean</span></span> | <span data-ttu-id="ed260-111">指示默认用户角色是否可以创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="ed260-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="ed260-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="ed260-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="ed260-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed260-113">Boolean</span></span> | <span data-ttu-id="ed260-114">指示默认用户角色是否可以创建安全组。</span><span class="sxs-lookup"><span data-stu-id="ed260-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="ed260-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="ed260-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="ed260-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed260-116">Boolean</span></span> | <span data-ttu-id="ed260-117">指示默认用户角色是否可以读取其他用户。</span><span class="sxs-lookup"><span data-stu-id="ed260-117">Indicates whether the default user role can read other users.</span></span> |  

## <a name="relationships"></a><span data-ttu-id="ed260-118">关系</span><span class="sxs-lookup"><span data-stu-id="ed260-118">Relationships</span></span>

<span data-ttu-id="ed260-119">无。</span><span class="sxs-lookup"><span data-stu-id="ed260-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed260-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed260-120">JSON representation</span></span>

<span data-ttu-id="ed260-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed260-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.defaultUserRolePermissions"
}-->

```json
{
  "allowedToCreateApps": true,
  "allowedToCreateSecurityGroups": true,
  "allowedToReadOtherUsers": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "defaultUserRolePermissions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


