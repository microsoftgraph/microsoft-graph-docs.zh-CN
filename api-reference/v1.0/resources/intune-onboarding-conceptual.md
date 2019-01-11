---
title: 在 Intune 中注册设备以进行管理
description: " (BYOD) 注册允许用户注册其个人电话、 平板电脑或 Pc。 企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。"
localization_priority: Normal
ms.openlocfilehash: de2a87c08851081891ee641db50a4ca1c64cb314
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841319"
---
# <a name="enroll-devices-for-management-in-intune"></a>在 Intune 中注册设备以进行管理

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。

你可以通过 Microsoft Intune 注册设备（包括 Windows 电脑）以启用移动设备管理 (MDM)。 本主题介绍在 Intune 管理中注册移动设备的不同方法。 注册设备的方法取决于需要的设备类型、所有权和管理级别。 “自带设备”(BYOD) 注册可让用户注册其个人手机、平板电脑或电脑。 企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。

以下 Graph 资源可用于在 Intune 中管理注册：  

- [设备注册配置](intune-onboarding-deviceenrollmentconfiguration.md)
- [设备注册限制配置](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [设备注册平台限制](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [设备注册平台限制配置](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [设备注册 Windows Hello 企业版配置](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [设备管理 Exchange 连接器](intune-onboarding-devicemanagementexchangeconnector.md)
- [设备管理 exchange 连接器状态](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [设备管理 exchange 连接器同步类型](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [设备管理 exchange 连接器类型](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [设备管理合作伙伴](intune-onboarding-devicemanagementpartner.md)
- [设备管理合作伙伴应用程序类型](intune-onboarding-devicemanagementpartnerapptype.md)
- [设备管理合作伙伴租户状态](intune-onboarding-devicemanagementpartnertenantstate.md)
- [启用](intune-onboarding-enablement.md)
- [注册配置分配](intune-onboarding-enrollmentconfigurationassignment.md)
- [Intune 品牌](intune-onboarding-intunebrand.md)
- [MDM 证书颁发机构](intune-onboarding-mdmauthority.md)
- [移动威胁防护连接器](intune-onboarding-mobilethreatdefenseconnector.md)
- [移动威胁合作伙伴租户状态](intune-onboarding-mobilethreatpartnertenantstate.md)
- [本地条件访问设置](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [组织](intune-onboarding-organization.md)
- [RGB 颜色](intune-onboarding-rgbcolor.md)
- [VPP 令牌](intune-onboarding-vpptoken.md)
- [VPP 令牌状态](intune-onboarding-vpptokenstate.md)
- [VPP 令牌的同步状态](intune-onboarding-vpptokensyncstatus.md)
- [Windows Hello 业务 PIN 用法](intune-onboarding-windowshelloforbusinesspinusage.md)
