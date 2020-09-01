---
title: defaultUserRolePermissions 资源类型
description: 包含默认用户角色的某些可自定义权限。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca90884220f65bca752fcabe2e0ffe37578cdf90
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319693"
---
# <a name="defaultuserrolepermissions-resource-type"></a><span data-ttu-id="6502f-103">defaultUserRolePermissions 资源类型</span><span class="sxs-lookup"><span data-stu-id="6502f-103">defaultUserRolePermissions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6502f-104">包含在 Azure AD 中 certains 可自定义的默认用户角色的权限。</span><span class="sxs-lookup"><span data-stu-id="6502f-104">Contains certains customizable permissions of default user role in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="6502f-105">属性</span><span class="sxs-lookup"><span data-stu-id="6502f-105">Properties</span></span>

| <span data-ttu-id="6502f-106">属性</span><span class="sxs-lookup"><span data-stu-id="6502f-106">Property</span></span> | <span data-ttu-id="6502f-107">类型</span><span class="sxs-lookup"><span data-stu-id="6502f-107">Type</span></span> | <span data-ttu-id="6502f-108">说明</span><span class="sxs-lookup"><span data-stu-id="6502f-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="6502f-109">allowedToCreateApps</span><span class="sxs-lookup"><span data-stu-id="6502f-109">allowedToCreateApps</span></span> | <span data-ttu-id="6502f-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="6502f-110">Boolean</span></span> | <span data-ttu-id="6502f-111">指示默认用户角色是否可以创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="6502f-111">Indicates whether the default user role can create applications.</span></span> |  
| <span data-ttu-id="6502f-112">allowedToCreateSecurityGroups</span><span class="sxs-lookup"><span data-stu-id="6502f-112">allowedToCreateSecurityGroups</span></span> | <span data-ttu-id="6502f-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6502f-113">Boolean</span></span> | <span data-ttu-id="6502f-114">指示默认用户角色是否可以创建安全组。</span><span class="sxs-lookup"><span data-stu-id="6502f-114">Indicates whether the default user role can create security groups.</span></span> |  
| <span data-ttu-id="6502f-115">allowedToReadOtherUsers</span><span class="sxs-lookup"><span data-stu-id="6502f-115">allowedToReadOtherUsers</span></span> | <span data-ttu-id="6502f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6502f-116">Boolean</span></span> | <span data-ttu-id="6502f-117">指示默认用户角色是否可以读取其他用户。</span><span class="sxs-lookup"><span data-stu-id="6502f-117">Indicates whether the default user role can read other users.</span></span> |  

## <a name="relationships"></a><span data-ttu-id="6502f-118">关系</span><span class="sxs-lookup"><span data-stu-id="6502f-118">Relationships</span></span>

<span data-ttu-id="6502f-119">无。</span><span class="sxs-lookup"><span data-stu-id="6502f-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6502f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6502f-120">JSON representation</span></span>

<span data-ttu-id="6502f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6502f-121">The following is a JSON representation of the resource.</span></span>

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
