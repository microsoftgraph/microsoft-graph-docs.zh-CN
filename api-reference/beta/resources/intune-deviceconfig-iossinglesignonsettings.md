---
title: iosSingleSignOnSettings 资源类型
description: 单一登录的 iOS Kerberos 身份验证设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 20c6cabbd5f18349058c68136052c8d56894dccc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728561"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="d41f0-103">iosSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d41f0-103">iosSingleSignOnSettings resource type</span></span>

<span data-ttu-id="d41f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d41f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d41f0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d41f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d41f0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d41f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d41f0-107">单一登录的 iOS Kerberos 身份验证设置</span><span class="sxs-lookup"><span data-stu-id="d41f0-107">iOS Kerberos authentication settings for single sign-on</span></span>

## <a name="properties"></a><span data-ttu-id="d41f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="d41f0-108">Properties</span></span>
|<span data-ttu-id="d41f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="d41f0-109">Property</span></span>|<span data-ttu-id="d41f0-110">类型</span><span class="sxs-lookup"><span data-stu-id="d41f0-110">Type</span></span>|<span data-ttu-id="d41f0-111">说明</span><span class="sxs-lookup"><span data-stu-id="d41f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d41f0-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="d41f0-112">allowedAppsList</span></span>|<span data-ttu-id="d41f0-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d41f0-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d41f0-114">允许使用此登录名的应用程序标识符列表。</span><span class="sxs-lookup"><span data-stu-id="d41f0-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="d41f0-115">如果省略此字段，则登录将应用于设备上的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="d41f0-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="d41f0-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d41f0-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d41f0-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="d41f0-117">allowedUrls</span></span>|<span data-ttu-id="d41f0-118">String collection</span><span class="sxs-lookup"><span data-stu-id="d41f0-118">String collection</span></span>|<span data-ttu-id="d41f0-119">必须匹配才能使用此登录的 HTTP Url 的列表。</span><span class="sxs-lookup"><span data-stu-id="d41f0-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="d41f0-120">对于 iOS 9.0 或更高版本，可以使用通配符。</span><span class="sxs-lookup"><span data-stu-id="d41f0-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="d41f0-121">displayName</span><span class="sxs-lookup"><span data-stu-id="d41f0-121">displayName</span></span>|<span data-ttu-id="d41f0-122">String</span><span class="sxs-lookup"><span data-stu-id="d41f0-122">String</span></span>|<span data-ttu-id="d41f0-123">在接收设备上显示的登录设置的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d41f0-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="d41f0-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d41f0-124">kerberosPrincipalName</span></span>|<span data-ttu-id="d41f0-125">String</span><span class="sxs-lookup"><span data-stu-id="d41f0-125">String</span></span>|<span data-ttu-id="d41f0-126">Kerberos 主体名称。</span><span class="sxs-lookup"><span data-stu-id="d41f0-126">A Kerberos principal name.</span></span> <span data-ttu-id="d41f0-127">如果未提供，则在配置文件安装过程中系统会提示用户一个。</span><span class="sxs-lookup"><span data-stu-id="d41f0-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="d41f0-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="d41f0-128">kerberosRealm</span></span>|<span data-ttu-id="d41f0-129">String</span><span class="sxs-lookup"><span data-stu-id="d41f0-129">String</span></span>|<span data-ttu-id="d41f0-130">Kerberos 领域名称。</span><span class="sxs-lookup"><span data-stu-id="d41f0-130">A Kerberos realm name.</span></span> <span data-ttu-id="d41f0-131">区分大小写。</span><span class="sxs-lookup"><span data-stu-id="d41f0-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d41f0-132">关系</span><span class="sxs-lookup"><span data-stu-id="d41f0-132">Relationships</span></span>
<span data-ttu-id="d41f0-133">无</span><span class="sxs-lookup"><span data-stu-id="d41f0-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d41f0-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d41f0-134">JSON Representation</span></span>
<span data-ttu-id="d41f0-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d41f0-135">Here is a JSON representation of the resource.</span></span>
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





