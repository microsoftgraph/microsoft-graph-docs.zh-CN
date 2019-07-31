---
title: iosSingleSignOnSettings 资源类型
description: 单一登录的 iOS Kerberos 身份验证设置
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c68683d5152657fedbd6ac04d191bae104849a8c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001122"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="4854a-103">iosSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4854a-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="4854a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4854a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4854a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4854a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4854a-106">单一登录的 iOS Kerberos 身份验证设置</span><span class="sxs-lookup"><span data-stu-id="4854a-106">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="4854a-107">属性</span><span class="sxs-lookup"><span data-stu-id="4854a-107">Properties</span></span>
|<span data-ttu-id="4854a-108">属性</span><span class="sxs-lookup"><span data-stu-id="4854a-108">Property</span></span>|<span data-ttu-id="4854a-109">类型</span><span class="sxs-lookup"><span data-stu-id="4854a-109">Type</span></span>|<span data-ttu-id="4854a-110">说明</span><span class="sxs-lookup"><span data-stu-id="4854a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4854a-111">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="4854a-111">allowedAppsList</span></span>|<span data-ttu-id="4854a-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4854a-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4854a-113">允许使用此登录名的应用程序标识符列表。</span><span class="sxs-lookup"><span data-stu-id="4854a-113">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="4854a-114">如果省略此字段, 则登录将应用于设备上的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="4854a-114">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="4854a-115">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4854a-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4854a-116">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="4854a-116">allowedUrls</span></span>|<span data-ttu-id="4854a-117">String collection</span><span class="sxs-lookup"><span data-stu-id="4854a-117">String collection</span></span>|<span data-ttu-id="4854a-118">必须匹配才能使用此登录的 HTTP Url 的列表。</span><span class="sxs-lookup"><span data-stu-id="4854a-118">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="4854a-119">对于 iOS 9.0 或更高版本, 可以使用通配符。</span><span class="sxs-lookup"><span data-stu-id="4854a-119">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="4854a-120">displayName</span><span class="sxs-lookup"><span data-stu-id="4854a-120">displayName</span></span>|<span data-ttu-id="4854a-121">String</span><span class="sxs-lookup"><span data-stu-id="4854a-121">String</span></span>|<span data-ttu-id="4854a-122">在接收设备上显示的登录设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4854a-122">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="4854a-123">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4854a-123">kerberosPrincipalName</span></span>|<span data-ttu-id="4854a-124">String</span><span class="sxs-lookup"><span data-stu-id="4854a-124">String</span></span>|<span data-ttu-id="4854a-125">Kerberos 主体名称。</span><span class="sxs-lookup"><span data-stu-id="4854a-125">A Kerberos principal name.</span></span> <span data-ttu-id="4854a-126">如果未提供, 则在配置文件安装过程中系统会提示用户一个。</span><span class="sxs-lookup"><span data-stu-id="4854a-126">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="4854a-127">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="4854a-127">kerberosRealm</span></span>|<span data-ttu-id="4854a-128">String</span><span class="sxs-lookup"><span data-stu-id="4854a-128">String</span></span>|<span data-ttu-id="4854a-129">Kerberos 领域名称。</span><span class="sxs-lookup"><span data-stu-id="4854a-129">A Kerberos realm name.</span></span> <span data-ttu-id="4854a-130">区分大小写。</span><span class="sxs-lookup"><span data-stu-id="4854a-130">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4854a-131">关系</span><span class="sxs-lookup"><span data-stu-id="4854a-131">Relationships</span></span>
<span data-ttu-id="4854a-132">无</span><span class="sxs-lookup"><span data-stu-id="4854a-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4854a-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4854a-133">JSON Representation</span></span>
<span data-ttu-id="4854a-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4854a-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosSingleSignOnSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosSingleSignOnSettings",
  "allowedAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "allowedUrls": [
    "String"
  ],
  "displayName": "String",
  "kerberosPrincipalName": "String",
  "kerberosRealm": "String"
}
```





