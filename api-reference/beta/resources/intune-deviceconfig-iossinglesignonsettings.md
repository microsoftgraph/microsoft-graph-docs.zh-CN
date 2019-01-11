---
title: iosSingleSignOnSettings 资源类型
description: iOS 的单一登录的 Kerberos 身份验证设置
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 17c2e100f9762334173ca6ca7049d1e5933f8616
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841060"
---
# <a name="iossinglesignonsettings-resource-type"></a><span data-ttu-id="4c391-103">iosSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c391-103">iosSingleSignOnSettings resource type</span></span>

> <span data-ttu-id="4c391-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4c391-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c391-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4c391-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c391-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4c391-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c391-107">iOS 的单一登录的 Kerberos 身份验证设置</span><span class="sxs-lookup"><span data-stu-id="4c391-107">iOS Kerberos authentication settings for single sign-on</span></span>
## <a name="properties"></a><span data-ttu-id="4c391-108">属性</span><span class="sxs-lookup"><span data-stu-id="4c391-108">Properties</span></span>
|<span data-ttu-id="4c391-109">属性</span><span class="sxs-lookup"><span data-stu-id="4c391-109">Property</span></span>|<span data-ttu-id="4c391-110">类型</span><span class="sxs-lookup"><span data-stu-id="4c391-110">Type</span></span>|<span data-ttu-id="4c391-111">Description</span><span class="sxs-lookup"><span data-stu-id="4c391-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c391-112">allowedAppsList</span><span class="sxs-lookup"><span data-stu-id="4c391-112">allowedAppsList</span></span>|<span data-ttu-id="4c391-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c391-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4c391-114">允许使用此登录名的应用程序标识符的列表。</span><span class="sxs-lookup"><span data-stu-id="4c391-114">List of app identifiers that are allowed to use this login.</span></span> <span data-ttu-id="4c391-115">如果省略此字段，则在登录适用于设备上的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="4c391-115">If this field is omitted, the login applies to all applications on the device.</span></span> <span data-ttu-id="4c391-116">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="4c391-116">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4c391-117">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="4c391-117">allowedUrls</span></span>|<span data-ttu-id="4c391-118">String 集合</span><span class="sxs-lookup"><span data-stu-id="4c391-118">String collection</span></span>|<span data-ttu-id="4c391-119">必须匹配才能使用此登录名的 HTTP Url 的列表。</span><span class="sxs-lookup"><span data-stu-id="4c391-119">List of HTTP URLs that must be matched in order to use this login.</span></span> <span data-ttu-id="4c391-120">与 iOS 9.0 或更高版本中，可以使用通配符。</span><span class="sxs-lookup"><span data-stu-id="4c391-120">With iOS 9.0 or later, a wildcard characters may be used.</span></span>|
|<span data-ttu-id="4c391-121">displayName</span><span class="sxs-lookup"><span data-stu-id="4c391-121">displayName</span></span>|<span data-ttu-id="4c391-122">字符串</span><span class="sxs-lookup"><span data-stu-id="4c391-122">String</span></span>|<span data-ttu-id="4c391-123">接收设备上显示的登录设置显示名称。</span><span class="sxs-lookup"><span data-stu-id="4c391-123">The display name of login settings shown on the receiving device.</span></span>|
|<span data-ttu-id="4c391-124">kerberosPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4c391-124">kerberosPrincipalName</span></span>|<span data-ttu-id="4c391-125">字符串</span><span class="sxs-lookup"><span data-stu-id="4c391-125">String</span></span>|<span data-ttu-id="4c391-126">Kerberos 的主体名称。</span><span class="sxs-lookup"><span data-stu-id="4c391-126">A Kerberos principal name.</span></span> <span data-ttu-id="4c391-127">如果未提供，一个配置文件安装过程中提示用户。</span><span class="sxs-lookup"><span data-stu-id="4c391-127">If not provided, the user is prompted for one during profile installation.</span></span>|
|<span data-ttu-id="4c391-128">kerberosRealm</span><span class="sxs-lookup"><span data-stu-id="4c391-128">kerberosRealm</span></span>|<span data-ttu-id="4c391-129">字符串</span><span class="sxs-lookup"><span data-stu-id="4c391-129">String</span></span>|<span data-ttu-id="4c391-130">Kerberos 领域名。</span><span class="sxs-lookup"><span data-stu-id="4c391-130">A Kerberos realm name.</span></span> <span data-ttu-id="4c391-131">区分大小写。</span><span class="sxs-lookup"><span data-stu-id="4c391-131">Case sensitive.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c391-132">Relationships</span><span class="sxs-lookup"><span data-stu-id="4c391-132">Relationships</span></span>
<span data-ttu-id="4c391-133">无</span><span class="sxs-lookup"><span data-stu-id="4c391-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c391-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c391-134">JSON Representation</span></span>
<span data-ttu-id="4c391-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c391-135">Here is a JSON representation of the resource.</span></span>
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





