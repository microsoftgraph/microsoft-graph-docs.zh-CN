---
title: 使用 Intune 载入托管设备 - Microsoft Graph API
description: 列出用于为租户Graph载入 (配置和) 设备的适用于 Intune 终结点的 Microsoft (API) REST 应用程序。
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
ms.openlocfilehash: 75d06ef328c6af99eaba70df8b0d3fd858921bd1
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63367739"
---
# <a name="enroll-devices-for-management-in-intune"></a>在 Intune 中注册设备以进行管理

命名空间：microsoft.graph

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

你可以通过 Microsoft Intune 注册设备（包括 Windows 电脑）以启用移动设备管理 (MDM)。 本主题介绍在 Intune 管理中注册移动设备的不同方法。 注册设备的方法取决于需要的设备类型、所有权和管理级别。 “自带设备”(BYOD) 注册可让用户注册其个人手机、平板电脑或电脑。 企业拥有设备 (COD) 注册允许管理场景，例如远程擦除、共享设备或设备的用户相关性。

以下 Graph 资源可用于在 Intune 中管理注册：

- [证书连接器设置](intune-onboarding-certificateconnectorsetting.md)
- [合规性管理合作伙伴](intune-onboarding-compliancemanagementpartner.md)
- [合规性管理合作伙伴分配](intune-onboarding-compliancemanagementpartnerassignment.md)
- [设备和应用管理数据](intune-onboarding-deviceandappmanagementdata.md)
- [设备共同管理颁发机构配置](intune-onboarding-devicecomanagementauthorityconfiguration.md)
- [设备注册配置类型](intune-onboarding-deviceenrollmentconfigurationtype.md)
- [设备注册限制配置](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [设备注册平台限制](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [设备注册平台限制配置](intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)
- [设备注册平台限制配置](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [设备注册 Windows Hello 企业版配置](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [设备管理 Exchange 访问级别](intune-onboarding-devicemanagementexchangeaccesslevel.md)
- [设备管理 Exchange 访问规则](intune-onboarding-devicemanagementexchangeaccessrule.md)
- [设备管理 Exchange 访问规则类型](intune-onboarding-devicemanagementexchangeaccessruletype.md)
- [设备管理 Exchange 连接器](intune-onboarding-devicemanagementexchangeconnector.md)
- [设备管理 Exchange 连接器状态](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [设备管理 Exchange 连接器同步类型](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [设备管理 Exchange 连接器类型](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [设备管理 Exchange 设备类](intune-onboarding-devicemanagementexchangedeviceclass.md)
- [设备管理 Exchange 本地策略](intune-onboarding-devicemanagementexchangeonpremisespolicy.md)
- [设备管理合作伙伴](intune-onboarding-devicemanagementpartner.md)
- [设备管理合作伙伴应用类型](intune-onboarding-devicemanagementpartnerapptype.md)
- [设备管理合作伙伴分配](intune-onboarding-devicemanagementpartnerassignment.md)
- [设备管理合作伙伴租户状态](intune-onboarding-devicemanagementpartnertenantstate.md)
- [设备平台类型](intune-onboarding-deviceplatformtype.md)
- [注册配置分配](intune-onboarding-enrollmentconfigurationassignment.md)
- [注册限制平台类型](intune-onboarding-enrollmentrestrictionplatformtype.md)
- [Intune 品牌](intune-onboarding-intunebrand.md)
- [MDM 颁发机构](intune-onboarding-mdmauthority.md)
- [适用于企业的 Microsoft Store 门户选定内容的选项](intune-onboarding-microsoftstoreforbusinessportalselectionoptions.md)
- [移动威胁防护连接器](intune-onboarding-mobilethreatdefenseconnector.md)
- [移动威胁合作伙伴租户状态](intune-onboarding-mobilethreatpartnertenantstate.md)
- [本地条件访问设置](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [组织](intune-onboarding-organization.md)
- [侧加载密钥](intune-onboarding-sideloadingkey.md)
- [VPP 令牌](intune-onboarding-vpptoken.md)
- [VPP 令牌操作结果](intune-onboarding-vpptokenactionresult.md)
- [VPP 令牌许可证摘要](intune-onboarding-vpptokenlicensesummary.md)
- [VPP 令牌撤销许可证操作结果](intune-onboarding-vpptokenrevokelicensesactionresult.md)
- [VPP 令牌状态](intune-onboarding-vpptokenstate.md)
- [VPP 令牌同步状态](intune-onboarding-vpptokensyncstatus.md)
- [Windows 10 注册完成页配置](intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)
- [Windows Hello 企业版 PIN 使用情况](intune-onboarding-windowshelloforbusinesspinusage.md)
