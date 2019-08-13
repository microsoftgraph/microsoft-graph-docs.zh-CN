---
title: Microsoft Intune 中的共享资源-Microsoft Graph API
description: 列出支持租户组织的多个工作流的 Intune 终结点 (REST) 的 Microsoft Graph API。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: 0d2252093f222f5908756f312c2e82d591c29920
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372802"
---
# <a name="shared-resources-in-microsoft-intune"></a>Microsoft Intune 中的共享资源

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

这些终结点在多个 Microsoft Graph API for Intune 工作流中使用。  使用给定资源所需的意向、目的和权限因特定工作流和基础调用的上下文而异。  此外, 特定工作流仅支持某些方法、属性和操作。

以下关系图资源在 Intune 工作流之间共享:

- [操作状态](intune-shared-actionstate.md)
- [所有设备分配目标](intune-shared-alldevicesassignmenttarget.md)
- [所有许可的用户分配目标](intune-shared-alllicensedusersassignmenttarget.md)
- [符合性状态](intune-shared-compliancestatus.md)
- [设备和应用管理分配目标](intune-shared-deviceandappmanagementassignmenttarget.md)
- [设备应用管理](intune-shared-deviceappmanagement.md)
- [设备类别](intune-shared-devicecategory.md)
- [设备注册类型](intune-shared-deviceenrollmenttype.md)
- [设备管理](intune-shared-devicemanagement.md)
- [设备平台类型](intune-shared-deviceplatformtype.md)
- [设备类型](intune-shared-devicetype.md)
- [支持](intune-shared-enablement.md)
- [支持](intune-shared-enablement.md)
- [排除组分配目标](intune-shared-exclusiongroupassignmenttarget.md)
- [组分配目标](intune-shared-groupassignmenttarget.md)
- [安装意图](intune-shared-installintent.md)
- [IP 范围](intune-shared-iprange.md)
- [IPv4 范围](intune-shared-ipv4range.md)
- [IPv6 范围](intune-shared-ipv6range.md)
- [键/值对](intune-shared-keyvaluepair.md)
- [MIME 内容](intune-shared-mimecontent.md)
- [移动应用疑难解答事件](intune-shared-mobileapptroubleshootingevent.md)
- [代理域](intune-shared-proxieddomain.md)
- [Report](intune-shared-report.md)
- [报表根目录](intune-shared-reportroot.md)
- [生成的应用状态](intune-shared-resultantappstate.md)
- [RGB 颜色](intune-shared-rgbcolor.md)
- [运行状态](intune-shared-runstate.md)
- [保存的 UI 状态生成选项](intune-shared-saveduistategenerationoptions.md)
- [URI](intune-shared-uri.md)
- [用户](intune-shared-user.md)
- [VPP 令牌帐户类型](intune-shared-vpptokenaccounttype.md)
- [VPP 令牌操作失败原因](intune-shared-vpptokenactionfailurereason.md)
- [Windows 域加入配置](intune-shared-windowsdomainjoinconfiguration.md)
